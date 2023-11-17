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
                
                git url: 'https://github.com/binitapatel164/ecommerce.git', branch: 'main'
                
            }
        }

        stage('Unit Test') {
            steps {
               
                sh 'mvn test'
                
            }

        stage('Integration Test') {
            steps {
                // Run integration tests (if applicable)
                sh 'mvn integration-test' // Example command for Maven
            }
        }
        }
    }
}

