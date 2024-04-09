@Library("my-library") _

pipeline {
    agent any
    stages {
        stage('Login to Docker Hub') {
            steps {
                script {
                    // Pass Docker Hub credentials as parameters to the function
                    myStep('DockerUsername', 'DockerPassword')
                }
            }
        }
        // Add more stages as needed
    }
}
