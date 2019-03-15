pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('test') {
      agent any
      steps {
        sh 'echo "dockerimage created"'
      }
    }
  }
  environment {
    test = 'value'
  }
}