pipeline {
  agent {label 'agent1'} 
  tools {
    maven 'mymaven3.5'
  }

  options {
    skipDefaultCheckout()
  }
  
  stages {
    stage('Checkout') { 
      steps {
        echo "in checkout"
        //echo "sleep 120"
        // sh 'sleep 120'
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
