pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from Git
                git 'https://github.com/Shobana96/newproject.git'
            }
        }

        stage('Build') {
            steps {
                // Build the project with Maven
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                // Run tests (if applicable)
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                // Create Docker image and push to registry
                script {
                    // Docker commands
                }
            }
        }
    }

    post {
        success {
            // Actions to perform on success
        }
        failure {
            // Actions to perform on failure
        }
    }
}
