pipeline {
    agent {
        docker {
            image 'python:3.11-slim' // Specify a desired Python version
            label 'docker-build-agent'
        }
    }
    stages {
        stage('Install Dependencies and Run Tests') {
            steps {
                sh 'python --version'
                sh 'pip install -r requirements.txt'
                sh './run_tests.sh'
            }
        }
    }
}
