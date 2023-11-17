pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout the repository
                git url: 'https://github.com/binitapatel164/ecommerce.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                // Perform build steps here
                sh 'mvn clean package'

            }
        }

        stage('Unit Test') {
            steps {
                // Run unit tests for the application
                sh 'mvn test' // Example command for Maven
            }
        }

        stage('Deploy') {
            steps {
                // Deploy the application to a server 
                sh 'scp target/app.war user@your-server:/path/to/deploy' // Example command using SCP
            }
        }
        
        }
    }

