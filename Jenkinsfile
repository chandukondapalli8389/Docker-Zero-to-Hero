pipeline {
    agent any

    stages {
        stage("Build Docker image") {
            steps {
                script {
                    sh'''
                    cd examples/python-web-app
                    docker build -t python-web-app:latest .
                    '''
                }
            }
        }
        stage("Run Docker image") {
            steps {
                script {
                    sh'''
                    docker run -d -p 8001:8000 python-web-app:latest
                    '''
                }
            }
        }
    }  
}