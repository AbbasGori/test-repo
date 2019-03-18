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
        dockerfile {
          filename 'Dockerfile'
        }

      }
      steps {
        echo 'images'
        node(label: 's4-dev')
      }
    }
  }
}