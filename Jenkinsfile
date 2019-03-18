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
        echo 'hi'
        sh 'hostname -I'
        sh 'sudo docker build ~/ -t test'
      }
    }
    stage('next') {
      steps {
        sh 'echo ""'
      }
    }
  }
}