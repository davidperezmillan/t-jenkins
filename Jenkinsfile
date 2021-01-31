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

        stage('Info JAVA Version') {
          agent {
            docker {
              image 'openjdk:8-jre'
            }

          }
          steps {
            echo 'Hello, JDK'
            sh 'java -version'
          }
        }

      }
    }

  }
}