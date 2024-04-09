@Library("my-library") _

pipeline {
    agent any
    stages {
        stage('Login to Docker Hub') {
            steps {
                script {
                    myStep('DockerUsername', 'DockerPassword')
                }
            }
        }
    }
}

