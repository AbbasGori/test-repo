pipeline {
  agent {
    node {
      label 'master-jenkins'
    }

  }
  stages {
    stage('test') {
      agent {
        node {
          label 'master-jenkins'
        }

      }
      steps {
        sh 'hostname -I'
      }
    }
  }
}