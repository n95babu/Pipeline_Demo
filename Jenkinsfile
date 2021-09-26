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
          stage('Email') {
            steps {
                emailext (to: 'n95babu@gmail.com', subject: "Email Report from - '${env.JOB_NAME}' ", body: readFile("target/surefire-reports/emailable-report.html"), mimeType: 'text/html');
            }
        }
    }
}
