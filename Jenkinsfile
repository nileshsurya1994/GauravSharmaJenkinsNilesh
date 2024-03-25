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

        stage('Testing') {
            steps {
                echo 'Testing'
            }
        }
        
        
        stage('Environmental variables') {
            steps {
                sh 'echo "${USER}"'
                sh 'echo "${DATE}"'
                
            }
        }
        stage('Last STAge') {
            steps {
                echo 'Last STAge'
                
            }
        }
        stage('Run Commands') {
            environment{
            pass = 'Ramraja'
        }
        
            steps {
                echo "Hare Ram"
               
                sh '''
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
                echo '.......failure is not good......'
                 }
                 success {
                echo '.......success......'
                 }
        }
}
