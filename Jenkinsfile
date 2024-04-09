@Library("my-library") _

pipeline {
    agent any
    parameters {
        string(name: 'DOCKER_USERNAME', defaultValue: '', description: 'Docker Hub Username')
        string(name: 'DOCKER_PASSWORD', defaultValue: '', description: 'Docker Hub Password')
    }
    stages {
        stage('Login to Docker Hub') {
            steps {
                script {
                    DockerUtils.loginToDockerHub(params.DOCKER_USERNAME, params.DOCKER_PASSWORD)
                }
            }
        }
        // Add more stages as needed
    }
}


