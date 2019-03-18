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
          label 's4-dev'
        }

      }
      steps {
        sh 'echo completed'
      }
    }
  }
}