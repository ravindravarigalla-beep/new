pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh '''
                   curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
                   unzip awscliv2.zip
                   ./aws/install
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
