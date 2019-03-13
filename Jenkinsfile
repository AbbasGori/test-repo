pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        build 'html'
      }
    }
  }
  environment {
    test = 'value'
  }
}