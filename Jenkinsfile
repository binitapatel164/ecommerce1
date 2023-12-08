pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control (e.g., Git)
                git 'https://github.com/binitapatel164/ecommerce1.git'
            }
        }

        stage('Build') {
            steps {
                bat 'echo "Building..."'
            }
        }

        stage('Unit Test') {
            steps {
               bat 'Unit test'
            }
        }

        stage('Integration Test') {
            steps {
                bat 'test'
            }
        }

        stage('Deploy') {
            steps {
                bat 'deploy'
        }


    }

}
