pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/your-username/Jenkins-Project.git'
            }
        }

        stage('Build') {
            steps {
                sh 'docker-compose build'
            }
        }

        stage('Deploy') {
            steps {
                sh 'docker-compose down || true'
                sh 'docker-compose up -d'
            }
        }
    }
}