pipeline {
    agent any

    stages {
        stage("Build Docker image") {
            steps {
                script {
                    sh'''
                    whoami
                   cd examples/python-web-app
                   docker build -t python-web-app:latest .
                    '''
                }
            }
        }
    }  
}