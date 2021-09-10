pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo 'Building...'
            }
        }
        stage('Test') { 
            steps {
                echo 'Testing...'
            }
        }
          stage('SonarQube analysis') { 
            steps {
                echo 'SonarQube analysis...'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'Deploying...' 
            }
        }
        stage('Releasing'){
        steps {
                echo 'Releasing...' 
         }
       }
    }
}
