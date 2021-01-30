pipeline {
  agent {
    docker {
      image 'nonave/eureka:latest'
      args '--network microservicios_docker-microservices-network'
    }

  }
  stages {
    stage('Test') {
      steps {
        sh 'mvn --version'
      }
    }

  }
}