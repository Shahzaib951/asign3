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
                bat 'echo Building the application'
                bat 'dir' // List files in the workspace directory for debugging
                bat 'python app.py'
            }
        }
    }
}
