pipeline {
    agent any
    stages {
        stage('Login to Docker Hub') {
            steps {
                script {
                    loginToDockerHub('username', 'password')
                }
            }
        }
    }
}


