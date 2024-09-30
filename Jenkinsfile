pipeline {
    agent any
    stages {
        stage('Clone') {
            steps {
                echo 'Clone...'
                git branch: 'main', url: 'https://github.com/vahtyah/Jenkins.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Các bước build
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Các bước kiểm thử
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to Staging...'
                // Các bước deploy đến staging

            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Deploying to Production...'
                // Các bước deploy đến production

            }
        }
    }
}
