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
                sh 'echo "Building..."'
            }
        }

        stage('Unit Test') {
            steps {
               sh 'Unit test'
            }
        }

        stage('Integration Test') {
            steps {
                sh 'test'
            }
        }

        stage('Deploy') {
            steps {
                sh 'deploy'
        }


    }

}
