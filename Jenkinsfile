pipeline {
  agent {
    docker {
      args '--network microservicios_docker-microservices-network'
      image 'eureka'
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