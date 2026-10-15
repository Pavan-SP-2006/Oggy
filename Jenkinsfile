
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'GitHub repository connected!'
            }
        }

        stage('Build Website') {
            steps {
                bat 'if exist index.html (echo index.html found) else (exit 1)'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t oggy-website:latest .'
            }
        }
    }
}
