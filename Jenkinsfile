pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }

  }
  stages {
    stage('docker') {
      agent {
        dockerfile {
          filename 'Dockerfile'
        }

      }
      steps {
        sleep 5
      }
    }
  }
}