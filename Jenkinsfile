pipeline {
  agent any
  stages {
    stage('test') {
      agent any
      steps {
        sh 'echo completed'
      }
    }
    stage('docker') {
      agent {
        docker {
          image 'jenkins'
        }

      }
      steps {
        echo 'images'
      }
    }
  }
}