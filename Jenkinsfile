pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control (e.g., Git)
                git url: 'https://github.com/binitapatel164/ecommerce1.git', branch: 'master'

            }
        }

        stage('Build') {
            steps {
                bat 'npm install'      // Install project dependencies
            }
        }

        stage('test') {
            steps{
                bat 'npm test'
            }
        }
        
        stage('Deploy') {
            steps {
                // Deploy the application to a server or cloud platform
                echo "scp target/app.war user@your-server:/path/to/deploy"
                // This is a placeholder, replace it with the actual deployment command
            }
        }

        stage('Quality Check') {
            steps {
                // Perform static code analysis, security scans, etc.
                echo "some_quality_check_command"
                // This is a placeholder, replace it with the actual quality check command
            }
        }
    }
}
