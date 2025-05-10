pipeline {
    agent {
        docker {
            image 'node:18'
        }
    }

    stages {
        stage('Check Version') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed.'
        }
    }
}

