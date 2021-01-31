pipeline {
  agent none
  stages {
    stage('Info') {
      parallel {
        stage('info Maven version') {
          agent {
            docker {
              image 'davidperez01/jenkins'
            }

          }
          steps {
            echo 'Hello, Maven'
            sh 'mvn --version'
          }
        }

        stage('Info JAVA version') {
          agent {
            docker {
              image 'davidperez01/jenkins'
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