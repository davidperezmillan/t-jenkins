pipeline {
  agent {
    docker {
      args '--network microservicios_docker-microservices-network'
      image 'nonave/eureka:latest'
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