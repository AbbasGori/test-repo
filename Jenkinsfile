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
        sh 'sudo docker build /home/abbasg/ -t dev-test'
      }
    }
    stage('next') {
      steps {
        sh 'echo "image created"'
      }
    }
  }
}