node {
  
  stages {
        stage('Start Docker Compose') {
                sh '''
                    echo "Starting Docker Compose"
                    docker-compose up -d
                '''
        }
    }

  
  
  stage('Test') {
     sh 'curl localhost:9000'
  }

}

