pipeline {
  agent {
    docker {
      args '--network microservicios_docker-microservices-network'
      image 'nonave:eureka'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean install'
      }
    }

  }
}