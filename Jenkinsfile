pipeline {
    agent any
    
    stages {
        stage('Checkout Git') {
            steps {
                git url:'https://github.com/32dc/dc32.git'    
            }
        } 
        stage('Echo') {
           steps {
               echo 'Running...'
           }
        }        
    }
}    
