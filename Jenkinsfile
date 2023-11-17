pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control (e.g., Git)
                git 'https://github.com/binitapatel164/ecommerce1'
            }
        }

        stage('Build') {
            steps {
                // Build your application (e.g., using Maven, Gradle, etc.)
                bat 'mvn clean package' // Example command for Maven
            }
        }

        stage('Unit Test') {
            steps {
                // Run unit tests for the application
                bat 'mvn test' // Example command for Maven
            }
        }

        stage('Integration Test') {
            steps {
                // Run integration tests (if applicable)
                bat 'mvn integration-test' // Example command for Maven
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application to a server or cloud platform
                bat 'scp target/app.war user@your-server:/path/to/deploy' // Example command using SCP
            }
        }

        stage('Quality Check') {
            steps {
                // Perform static code analysis, security scans, etc.
                bat 'some_quality_check_command' // Replace with actual command
            }
        }

        
    }

    
}

