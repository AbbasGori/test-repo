pipeline {
  agent {
    node {
      label 's4-dev'
    }

  }
  stages {
    stage('test') {
      agent any
      steps {
        sh 'echo completed'
      }
    }
    stage('docker') {
      agent {
        dockerfile {
          filename 'Dockerfile'
        }

      }
      steps {
        echo 'images'
      }
    }
  }
}