node {
  
  stage('Start Docker Compose') {
      sh 'docker-compose -f /home/Valentin/app-php/docker-compose.yaml up -d'
        }

  stage('Test') {
     sh 'curl localhost:9000'
  }

}

