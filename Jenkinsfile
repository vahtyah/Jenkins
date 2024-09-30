pipeline {
    agent any
    post {
        failure {
                echo "Это будет выполняться, если задача провалилась"
                mail to: 'vahtyah@gmail.com',
                    subject: "${env.JOB_NAME} – Сборка № ${env.BUILD_NUMBER} провалилась",
                    body: "Для получения дополнительной информации о провале пайплайна, проверьте консольный вывод по адресу ${env.BUILD_URL}.",
        }
    }
    
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
