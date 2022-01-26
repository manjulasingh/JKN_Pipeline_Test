pipeline {
    agent {
        docker {
            image 'python:3.10.1-alpine'
        }
    }
    stages {
        stage('Build') {
            steps {
                 echo "Hiii"
            }
        }
        stage('Test') {
            steps {
                echo "Hi"
            }
            post {
                always {
                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
        stage('Deliver') { 
            steps {
                echo "Hello" 
            }
        }
    }
}
