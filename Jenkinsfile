pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('docker') {
      steps {
        sleep 5
      }
    }
  }
  environment {
    test = 'value'
  }
}