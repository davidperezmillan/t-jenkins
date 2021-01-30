pipeline {
  agent none
  stages {
    stage('Info') {
      parallel {
        stage('info maven') {
          agent any
          steps {
            sh 'mvn --version'
          }
        }

        stage('info version') {
          agent any
          steps {
            sh 'mvn --version'
          }
        }

      }
    }

  }
}