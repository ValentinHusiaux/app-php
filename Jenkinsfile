node {
  
 stage('Start Docker Compose') {
     sh '''
           COMPOSE_FILE_PATH="$(pwd)/docker-compose.yaml"
           docker-compose -f $COMPOSE_FILE_PATH up -d
        '''
            }
  stage('Test') {
     sh 'curl localhost:9000'
  }

}

