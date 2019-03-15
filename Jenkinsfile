pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('test') {
      steps {
        sh 'echo "dockerimage created"'
      }
    }
  }
  environment {
    test = 'value'
  }
}