stage('Deploy to Kubernetes') {
    steps {
        bat 'kubectl apply -f deployment.yaml --validate=false'
    }
}