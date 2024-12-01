pipeline {
    agent any
    tools {
        nodejs 'NodeJs' // Ensure this matches the name in Jenkins configuration
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                bat 'npm install'
            }
        }
        stage('Test') {
            steps {
                bat 'npm test -- --passWithNoTests'
            }
        }
    }
}
