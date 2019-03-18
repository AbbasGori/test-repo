pipeline {
  agent any
  stages {
    stage('test') {
      agent {
        node {
          label 's4-dev'
        }

      }
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
        node(label: 's4-dev')
      }
    }
  }
}