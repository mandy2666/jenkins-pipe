@Library('my-library') _

pipeline {
    agent any

    parameters {
        string(name: 'DOCKER_USERNAME', description: 'Docker username')
        string(name: 'DOCKER_PASSWORD', defaultValue: '', description: 'Enter your Docker password', trim: true)
    }

    stages {
        stage('Docker Login') {
            steps {
                script {
                    DockerUtils(params.DOCKER_USERNAME, params.DOCKER_PASSWORD)
                }
            }
        }
    }
}




