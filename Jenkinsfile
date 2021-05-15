pipeline {
    agent { label 'jnlp-slave' }
    
    stages {
        stage('Checkout Git') {
            steps {
                git url:'https://github.com/32dc/dc32.git'    
            }
        }        
        stage('Main') {
            steps {
                script {
                    sh label: '', script: 'kubectl apply -f pod.yml'
                }    
            }
        }
    }
}    
