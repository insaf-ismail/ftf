pipeline {
    agent any
    stages {
        stage('clone repo') {
            steps { 
               git credentialsID: 'git_credentialsID', url='git@github.com:insaf-ismail/ftf.git'
            }
        }
      stage('build image') {
            steps { 
                echo 'sh "docker build -t insafdocker/ftf:latest"'
            }
        }
      stage('deploiment') {
            steps { 
                echo 'Welcome to LambdaTest'
            }
        }
    }
}
