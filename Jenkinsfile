pipeline {
    agent any

    stages {
        stage('Deploy Dashy') {
            steps {
                sh '''
                docker compose down || true
                docker compose pull
                docker compose up -d
                '''
            }
        }
    }
}
