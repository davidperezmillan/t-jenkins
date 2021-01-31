pipeline {
  agent {
    docker {
      image 'davidperez01/jenkins'
    }

  }
  stages {
    stage('Info') {
      parallel {
        stage('info Maven version') {
          agent any
          steps {
            echo 'Hello, Maven'
            sh 'mvn --version'
          }
        }

        stage('Info JAVA version') {
          agent any
          steps {
            echo 'Hello, JDK'
            sh 'java -version'
          }
        }

      }
    }

  }
}