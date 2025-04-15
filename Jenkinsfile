pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'docker build -t my-docker-image .'
            }
        }
        stage('Test') {
            steps {
                sh 'docker run my-docker-image'
            }
        }
    }
}
