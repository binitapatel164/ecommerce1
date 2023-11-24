pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Checkout code from version control
                git 'https://github.com/binitapatel164/ecommerce1.git'
            }
        }
        
        stage('Build') {
            steps {
                // Build the application 
                bat 'npm install' // or any build command relevant to your project
            }
        }
        
        stage('Test') {
            steps {
                // Run tests
                bat 'npm test'
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy the application
                bat 'npm run deploy' 
            }
        }
    }
    
   
}
