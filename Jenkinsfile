pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Retrieves the source code from the specified Git repository
                git 'https://github.com/binitapatel164/ecommerce1'
            }
        }

    stage('Build') {
            steps {
                // Builds the application
                sh 'mvn clean package' // Example command for Maven
            }
        }

        


    }


}
