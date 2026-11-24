pipeline {

    agent any

    environment {
        APP_NAME = 'MEDAD'
    }

    stages {

        stage('Build') {
            steps {
                echo "Building ${APP_NAME} - Webhook Test"
                sh 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                echo "Testing ${APP_NAME}"
                sh 'echo Tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${APP_NAME}"
                sh 'echo Deployment completed'
            }
        }

    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }

        failure {
            echo 'Pipeline failed'
        }
    }

}