pipeline {
    agent any
    stages {
       stage('Checkout-git'){
              steps {
               git poll: true, url: 'https://github.com/Criss091292/jenkins-CS.git'    
              }
       }
        stage('Install Requirements') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test App') { 
            steps {
                 sh 'npm test'
            }
        }
    }
}
