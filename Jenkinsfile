pipeline {
    agent {
        label 'windows' // Specify the Windows agent where Jenkins runs
    }
    stages {
        stage('Checkout') {
            steps {
                checkout scm // Pull the source code from your version control system (e.g., Git)
            }
        }
        
        stage('Build') {
            steps {
                bat 'npm install' // Build the solution using MSBuild
            }
        }
        
        stage('Unit Tests') {
            steps {
                bat 'npm start' // Run unit tests (replace YourTestFramework with your test runner)
            }
        }
        
        stage('Deploy') {
            steps {
                // Perform deployment steps here (e.g., copy artifacts to a server, publish to a web host, etc.)
                // You may use specific deployment tools or commands suitable for your ecommerce app
            }
        }
    }
}
