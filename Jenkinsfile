pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Checkout source code from version control (e.g., Git)
                git 'https://github.com/binitapatel164/ecommerce1'
            }
        }

    stage('Build') {
            steps {
                // Build your application (e.g., using Maven, Gradle, etc.)
                sh 'mvn clean package' // Example command for Maven
            }
        }

        


    }


}
