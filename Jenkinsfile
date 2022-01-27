pipeline {
    agent any
    stages {
        stage('clone repo') {
            steps { 
             
               sh"cd ftf"
            }
        }
      stage('build image') {
            steps { 
                 sh"cd ftf"
                 sh "ls"
                 sh "cd ftf"
                sh "cd ftf && sudo docker build -t insafdocker/ftf:latest ."
            }
      }
      stage('deploiment') {
            steps { 
                sh 'sudo docker run -p 8181:8181 -d insafdocker/ftf:latest'
            }
        }
    }
}
