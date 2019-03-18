pipeline {
  agent {
    node {
      label 'master-jenkins'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'hostname -I'
          }
        }
        stage('echo') {
          steps {
            sh 'echo in agent'
          }
        }
      }
    }
  }
}