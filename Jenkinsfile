pipeline {
  agent {label 'agent1'} 
  tools {
    maven 'mymaven3.5'
  }
  
  stages {
    stage('Checkout') { 
      steps {
        echo "no checkout"
        //git 'https://github.com/jyang49/multibranch.git'
      }
    }
    stage('Build') { 
      steps {
        sh 'mvn clean compile'
      }
    }
  }
}
