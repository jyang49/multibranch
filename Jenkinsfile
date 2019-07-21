pipeline {
  agent {label 'agent1'} 
  tools {
    maven 'mymaven3.5'
  }
  
  stages {
    stage('Checkout') { 
      steps {
        echo "in checkout"
        checkout scm
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
