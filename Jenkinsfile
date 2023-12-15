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

    }
}
