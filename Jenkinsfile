pipeline {
  agent none
  stages {
    stage('error') {
      agent any
      steps {
        sh 'mvn --version'
      }
    }

  }
}