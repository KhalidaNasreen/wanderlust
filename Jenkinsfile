pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Test') {
            steps {
                sh '''
                    cd backend
                    npm test -- --runInBand
                '''
            }
        }

        stage('Build') {
            steps {
                sh '''
                    docker compose build
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    docker compose down
                    docker compose up -d
                '''
            }
        }

        stage('Verify') {
            steps {
                sh '''
                    docker compose ps
                '''
            }
        }
    }

    post {
        success {
            echo 'Wanderlust CI/CD pipeline completed successfully!'
        }

        failure {
            echo 'Wanderlust CI/CD pipeline failed.'
        }
    }
}
