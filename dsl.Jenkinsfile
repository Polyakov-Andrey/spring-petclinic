pipeline {
   agent any
   environment { 
        CC = 'clang'
   }
   
   stages {
     stage('GIT') {
        steps {
           sh 'git --version'
           git 'https://github.com/Polyakov-Andrey/spring-petclinic.git'
        }    
     }
     stage('Build') {
       steps {
          echo 'Building..'
          sh label: 'Create jar', script: './mvnw package'
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
