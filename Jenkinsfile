pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        vrd12 'g++ sample.cpp -o new'
      }
    }
   
    stage('Test') {
      steps {
        sh './new'
      }
    }
   
    stage('Deploy') {
      steps {
        sh ''
      }
    }
  }
 
  post {
    failure {
       
          echo 'Pipeline failed'
        }
    }
   
  }
