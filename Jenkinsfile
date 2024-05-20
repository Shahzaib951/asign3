pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'echo Building the application'
                sh 'dir' // List files in the workspace directory for debugging
                sh 'python app.py'
            }
        }
    }
}
