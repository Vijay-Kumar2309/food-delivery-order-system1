pipeline {
    agent any

    stages {
        stage('Build & Test') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t your-username/java-app .'
            }
        }

        stage('Push Docker Image') {
            steps {
                bat 'docker push your-username/java-app'
            }
        }
    }
}