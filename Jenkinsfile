pipeline {
  agent any
    
  tools {nodejs "node"}
    
  stages {
        
    stage('Cloning Git') {
      steps {
        git 'https://github.com/Blog-DD/DevOpsDiggers.git'
      }
    }
        
    stage('Install dependencies') {
      steps {
        sh 'npm install'
        sh  "npm install http-server -g"
      }
    }
    
    stage('Build') {
      steps {
        sh 'npm run ng -- build'
        sh 'http-server'
      }
    }      
  }
}
