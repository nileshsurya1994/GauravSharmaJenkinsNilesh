pipeline {
    agent any

        environment{
            name = 'Ram'
        }
        parameters{
            string(name: 'person', defaultValue: 'Raja Ram', description: "lets gostring(name: 'person', defaultValue: 'Raja Ram', description: ")
            booleanParam(name :'color', defaultValue: true, description: "booleanParam(name :'color', defaultValue: true, description")
           choice(name: 'object', choices: ['red', 'hat', 'wine'], description: "choice(name: 'object', choices: ['red', 'hat', 'wine'], description")
        }
        
    stages {
        stage('Test') {
            steps {
                echo 'Test World'
                sh 'echo "${pass}"'
                sh 'echo "${person}"'
                sh 'echo "${ADULT}"'
                 sh 'echo "${PASSWORD}"'
                  sh 'echo "${object}"'
                  sh 'echo "${color}"'
            }
        }
        stage('Build') {
            steps {
                echo 'Build'
            }
        }
        stage('Continue???') {
            input {
                message "Should we continue?????"
                ok 'yes???'
            }
            steps {
                echo 'Deploy'
                sh 'pwd'
                sh 'echo "${name}"'
            }
        }
        
        stage('Environmental variables') {
            steps {
                sh 'echo "${USER}"'
                sh 'echo "${DATE}"'
                
            }
        }
        stage('Run Commands') {
            environment{
            pass = 'Ramraja'
        }
        
            steps {
                echo "Hare Ram"
                sh 'echo "${pass}"'
                sh '''
                date
                cal 2021
                pwd
                ls
                '''
            }
        }
        
    }
        
        post {
            always {
                echo 'alway run no matter what.............'
            }
                 failure {
                echo '.......failure......'
                 }
                 success {
                echo '.......success......'
                 }
        }
}
