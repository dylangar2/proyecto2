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
                bat 'docker push dylan226/proyecto2:ci'
            }
        }
    }
}
