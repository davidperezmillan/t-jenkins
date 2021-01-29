pipeline {
  agent {
    docker {
      image 'eureka'
      args '--network microservicios_docker-microservices-network'
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