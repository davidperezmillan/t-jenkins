pipeline {
  agent none
  stages {
    stage('error') {
      agent {
        node {
          label 'Main'
        }

      }
      steps {
        sh 'mvn --version'
      }
    }

  }
}