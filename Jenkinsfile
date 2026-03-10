pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Divyanshu-Developer-2004/DevOps-Training'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                if not exist C:\\deploy-demo mkdir C:\\deploy-demo
                copy index.html C:\\deploy-demo
                '''
            }
        }
    }
}