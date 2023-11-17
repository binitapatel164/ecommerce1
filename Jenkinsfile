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

        
        }
    }

