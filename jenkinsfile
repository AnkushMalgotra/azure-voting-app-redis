pipeline {
    agent any

    stages {
        stage('Verify Branch') {
            steps {
                // Echo the Git branch
                sh 'echo $GIT_BRANCH'
            }
        }

        stage('Docker Build') {
            steps {
                // Docker build using docker-compose
                sh 'docker-compose build'
            }
        }
    }
}
