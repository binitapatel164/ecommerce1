pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                // Your build commands (e.g., compiling, packaging)
                bat 'mvn clean install'
            }
        }
        
        
        
     
    }
    

}
