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
      }
    }
    
    stage('Build') {
      steps {
        sh 'npm run ng -- build'
      }
    }  
    
   stage('Test') {
      steps {
         sh 'npm test'
      }
    }      
  }
}
