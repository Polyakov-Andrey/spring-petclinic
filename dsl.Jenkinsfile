pipeline {
   agent any
   environment { 
        CC = 'clang'
   }
   
   stages {
     stage('GIT') {
        steps {
           sh 'git -version'
        }
     }
     stage('Build') {
       steps {
          echo 'Building..'
       }
     }
     stage('Test') {
       steps {
          echo 'Testing..'
       }
     }
     stage('Deploy') {
       steps {
           echo 'Deploying....'
       }
     }
   }
   /* insert Declarative Pipeline here */
}
