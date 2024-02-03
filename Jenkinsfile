pipeline {
    agent any
    environment {
        name = 'danish'
    }
    stages {
        stage('Run a command') {
            steps {
                sh '''
                ls
                date
                pwd cal 2025
                '''
            }
        }
         stage('Enviornment Variables') {
            steps {
                sh 'echo  "${BUILD_ID}"'
                sh 'echo  "${name}"'
            }
        }
         stage('Deploy on Test') {
            steps {
                echo 'deploy on test'
            }
        }
         stage('Deploy on Prod') {
            steps {
                echo 'deploy on Prod'
            }
        }
    }
    post{
        always {
            echo 'I will say hello again always be happy!'
        }
    }
}
