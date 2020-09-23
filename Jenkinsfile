pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh '''
                   aws --version
                   '''
            }
        }
        stage('Test') { 
            steps {
                sh '''
                   echo " hello world "
                   '''
            }
        }
        stage('Deploy') { 
            steps {
                sh "aws --version"
            }
        }
    }
}
