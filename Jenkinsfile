pipeline {
    agent any

    stages {
        stage('Build & Run Tests') {
            steps {
                bat 'mvn clean test'
            }
        }

        stage('Deploy to Kubernetes') {
            steps {
                bat 'kubectl apply -f deployment.yaml'
            }
        }
    }
}