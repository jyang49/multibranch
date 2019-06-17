pipeline {
  agent {label 'agent1'} 
  tools {
    maven 'mymaven3.5'
  }
  
  stages {
    stage('Check out') { 
      steps {
        git 'https://github.com/jyang49/multibranch.git'
      }
    }
    stage('Build') { 
      steps {
        sh 'mvn clean compile'
      }
    }
  }
}
