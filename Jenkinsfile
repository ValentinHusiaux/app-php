node {

 stage('Install Sudo') {
        
                sh 'apt-get update && apt-get install -y sudo'
        
        }


  stage('Install Docker Compose') {
                sh 'sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose'
                sh 'sudo chmod +x /usr/local/bin/docker-compose'
            }

  stage('Build') {

      sh 'docker-compose up -d'

        }
  stage('Test') {

     sh 'curl localhost:9000'

  }



}

