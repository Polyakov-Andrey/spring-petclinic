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
    }
    /* insert Declarative Pipeline here */
}
