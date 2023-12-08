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
                echo "Building..."
            }
        }

        stage('Unit Test') {
            steps {
               echo 'Unit test'
            }
        }

        stage('Integration Test') {
            steps {
                echo 'test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'deploy'
        }


    }

}
