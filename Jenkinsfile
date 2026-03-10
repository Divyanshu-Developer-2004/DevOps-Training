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
                if not exist D:\\Capgeminie\\DevOps\\demo1\\deploy-demo mkdir D:\\Capgeminie\\DevOps\\demo1\\deploy-demo
                copy hello.html D:\\Capgeminie\\DevOps\\demo1\\deploy-demo
                '''
            }
        }
    }
}