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
                echo "mvn clean package"; 
            }
        }

        stage('Unit Test') {
            steps {
                // Run unit tests for the application
                echo "mvn test"; 
            }
        }

        stage('Integration Test') {
            steps {
                // Run integration tests (if applicable)
                echo "mvn integration-test"; 
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application to a server or cloud platform
                echo "scp target/app.war user@your-server:/path/to/deploy"; 
            }
        }

        stage('Quality Check') {
            steps {
                // Perform static code analysis, security scans, etc.
                echo "some_quality_check_command"; 
            }
        }

        
    }

    
}
