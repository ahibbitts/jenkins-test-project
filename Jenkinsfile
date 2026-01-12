pipeline {
    agent any // Tells Jenkins to run the pipeline on any available agent
    stages {
        stage('Build') {
            steps {
                // A simple build step: print a message and run the python script
                echo 'Building the project...'
                sh 'python3 hello.py'
            }
        }
        stage('Test') {
            steps {
                // A simple test step: print a message
                echo 'Testing the project...'
                sh 'echo "Tests passed!"'
            }
        }
        stage('Deploy') {
            steps {
                // A simple deploy step: print a message
                echo 'Deploying the project...'
                sh 'echo "Deployment complete!"'
            }
        }
    }
}
