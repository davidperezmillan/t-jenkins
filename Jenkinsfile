pipeline {
  agent {
    docker {
      image 'nonave/eureka:latest'
      args '--network microservicios_docker-microservices-network'
    }

  }
  stages {
    stage('Print') {
      steps {
        echo 'Inicio de pipeline'
      }
    }

  }
}