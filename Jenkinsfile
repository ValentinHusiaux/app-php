pipeline {
    agent any
    stages {
        stage('version') {
            steps {
                sh 'docker-compose version'
            }
        stage('Build') {
            steps {
                sh 'docker-compose up -d'
            }
        stage('curl-create_db.php') {
            steps {
                sh 'curl localhost:9001/create_db.php'
            }
        stage('curl-create_table.php') {
            steps {
                sh 'curl localhost:9001/create_table.php'
            }
        stage('curl-getting_data.php') {
            steps {
                sh 'curl localhost:9001/getting_data.php'
            }
        stage('curl-insert_data.php') {
            steps {
                sh 'curl localhost:9001/insert_data.php'
            }
        stage('curl-remove_data.php') {
            steps {
                sh 'curl localhost:9001/remove_data.php'
            }
        stage('curl-remove_db.php') {
            steps {
                sh 'curl localhost:9001/remove_db.php'
            }
        }
    }
}
