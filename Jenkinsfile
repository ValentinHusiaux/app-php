node {
  
  stage('Start Docker Compose') {
      sh 'docker-compose up -d'
        }

  
  
  stage('Test') {
     sh 'curl localhost:9000'
  }

}

