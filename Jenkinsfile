pipeline {
    agent any

    stages {
        stage{"Build docker image"} {
           script {
               sh'''
                   cd examples/python-web-app
                   docker build -t python-web-app:latest .
                '''
           }
        }
    }
}