pipeline {
    environment{
        
    }
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "${DB_USER}"
                echo "${DB_PASSWORD}"
                echo "${DB_HOST}"
                echo "${DB_DATABASE}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'USER=${DB_USER}'
                sh 'echo "$USER"'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
