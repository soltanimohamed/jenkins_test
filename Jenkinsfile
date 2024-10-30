pipeline {
    agent any
    environment {
        BUILD_ENV = 'production'
    }
    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
            }
        }
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo "Deploying to ${BUILD_ENV} environment"
            }
        }
    }
    post {
        always {
            echo 'This will always run after each build!'
        }
        success {
            echo 'The build succeeded'
        }
        failure {
            echo 'The build failed!'
        }
    }
}