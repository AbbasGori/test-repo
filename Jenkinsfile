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
          agent {
            node {
              label 's4-dev'
            }

          }
          steps {
            sh 'hostname -I'
          }
        }
        stage('echo') {
          agent {
            node {
              label 's4-dev'
            }

          }
          steps {
            sh 'echo "in agent"'
          }
        }
      }
    }
    stage('next') {
      steps {
        sh 'echo ""'
      }
    }
  }
}