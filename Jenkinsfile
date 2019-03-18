pipeline {
  agent {
    node {
      label 'master-jenkins'
    }

  }
  stages {
    stage('test') {
      steps {
        sh 'hostname -I'
      }
    }
  }
}