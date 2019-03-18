pipeline {
  agent {
    node {
      label 's4-dev'
    }

  }
  stages {
    stage('test') {
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
        echo 'completed'
      }
    }
  }
}