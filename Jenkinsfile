pipeline {
    agent any

        environment{
            name = 'Ram'
        }
        
        
    stages {
        stage('Test') {
            steps {
                echo 'Test World'
                
                 
            }
        }
        stage('Build') {
            steps {
                echo 'Build'
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
