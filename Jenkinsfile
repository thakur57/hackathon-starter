pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/thakur57/hackathon-starter.git'
      }
    }
     
    stage('Build') {
      steps {
        sh 'npm install'
         sh 'npm start'
      }
    } 
    stages {
      stage('run docker file') {
        steps {
         sh ("sudo docker build -t thakur57/nodeapp:latest .")
        }
      }
    }
  }
}