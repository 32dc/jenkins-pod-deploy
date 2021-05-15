pipeline {
    agent { label 'jnlp-slave' }
    
    stages {
        stage('Checkout Git') {
            steps {
                git url:'https://github.com/32dc/dc32.git'    
            }
        }       
    }
}    
