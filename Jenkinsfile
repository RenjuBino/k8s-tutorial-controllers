pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                sh '''
                kubectl apply -f .
                sleep 60
                kubectl get services
                '''
            }
        }
    }
}