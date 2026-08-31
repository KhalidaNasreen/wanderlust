pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out Wanderlust project'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }

        stage('Build') {
            steps {
                echo 'Building Docker images'
            }
        }

        stage('Push') {
            steps {
                echo 'Pushing Docker images'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying Wanderlust application'
            }
        }
    }
}
