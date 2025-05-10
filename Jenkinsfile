pipeline {
    agent any

    stages {
        stage('Check Version') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example build command
                sh './build.sh'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example test command
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Example deploy command
                sh './deploy.sh'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}


