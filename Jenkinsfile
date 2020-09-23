pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh '''
                   curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
                   python get-pip.py
                   pip install awscli
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
