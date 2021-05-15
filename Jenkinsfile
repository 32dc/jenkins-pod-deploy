pipeline {
    agent {label 'jnlp-slave'}
    stages {
       stage('Echo') {
           steps {
               echo 'Stage: Echo'
               sleep 30
           }
        } 
       stage('Git Checkout') {
           steps {
               echo 'Stage: Git Checkout'
               sleep 10
               git branch: 'main', credentialsId: '4a0a0b13-b4c9-4a99-a64b-ecd948649d72', url: 'https://github.com/32dc/dc32.git' 
           }
        } 
       stage('Deploy Pod') {
           steps {
               echo 'Stage: Deploy Pod'
               sleep 10
               sh 'kubectl apply -f pod.yml'
           }
        }         
    }
} 
