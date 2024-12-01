pipeline {
    agent any
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
                // Added debug echo for clarity
                bat 'echo Running test script'
                
                // Use full path for bash executable and correct script path
                bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "C:/path/to/jenkins/scripts/test.sh"'
            }
        }
    }
}
