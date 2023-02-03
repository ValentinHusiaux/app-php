node {
  
 stage('Start Docker Compose') {
     sh '''
           echo "Getting the path of docker-compose.yaml"
           COMPOSE_FILE_PATH="$(pwd)/docker-compose.yaml"
           eho "Starting Docker Compose"
           docker-compose -f $COMPOSE_FILE_PATH up -d
        '''
            }
  stage('Test') {
     sh 'curl localhost:9000'
  }

}

