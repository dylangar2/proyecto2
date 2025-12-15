pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                bat 'docker-compose build'
            }
        }

        stage('Push Docker Image') {
    steps {
        bat '''
        docker tag proyecto2-ci-1-full:latest dylan226/proyecto2:ci
        docker push dylan226/proyecto2:ci
        '''
    }
}