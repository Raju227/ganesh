pipeline {
    agent any
    
    
    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/Raju227/ganesh.git'
            }
        }
        
        stage('Compile and Clean') { 
            steps {

                sh "mvn clean compile"
            }
        }
        stage('Test') { 
            steps {
                sh "mvn clean package"
            }
            
            
        }
        
        
    }
}
