node {
  
  stages {
        stage('Start Docker Compose') {
            steps {
                sh '''
                    echo "Starting Docker Compose"
                    docker-compose up -d
                '''
            }
        }
    }

  
  
  stage('Test') {
     sh 'curl localhost:9000'
  }

}

