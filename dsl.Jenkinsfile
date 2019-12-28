pipeline {
     agent none
     stages {
        stage('GIT') {
            // agent { docker 'maven:3-alpine' } 
            steps {
                echo 'Hello, Maven'
                sh 'git --version'
            }
        }
        stage('Example Test') {
            agent { docker 'openjdk:8-jre' } 
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
    /* insert Declarative Pipeline here */
}
