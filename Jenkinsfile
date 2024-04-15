@Library('my-library') _

pipeline {
    agent any

    parameters {
        string(name: 'DOCKER_USERNAME', description: 'Docker username')
        string(name: 'DOCKER_PASSWORD', description: 'Docker password', defaultValue: '', secret: true)
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



