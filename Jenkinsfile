pipeline {
    agent any
    stages {
        stage('clone repo') {
            steps { 
               git sh'git url'
            }
        }
      stage('build image') {
            steps { 
                sh "docker build -t insafdocker/ftf:latest"
            }
      }
      stage('deploiment') {
            steps { 
                sh 'here put the docker deployment'
            }
        }
    }
}
