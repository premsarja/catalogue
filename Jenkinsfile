pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo Installing JSlist"
                sh "npm i jslint"
                sh "echo starting lintchecks"
                sh "node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo linkchecks completed"
            }
        }
        stage('genearating Artifacts'){
          steps{
            sh "echo genrating Artifacts*********"
            sh "npm install && ls -ltr"

            }
        }
    }
}