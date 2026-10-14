
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'GitHub repository connected!'
            }
        }

        stage('Build') {
            steps {
                echo 'Building my DevOps project...'
                bat 'dir'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the website files...'
                bat 'if exist index.html (echo index.html found) else (exit 1)'
            }
        }
    }
}
