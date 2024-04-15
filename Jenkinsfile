// Importing global shared library
@Library('my-library') _

pipeline {
    agent any

    stages {
        stage('Docker Login') {
            steps {
                script {
                    // Using withCredentials to access Docker credentials
                    withCredentials([usernamePassword(credentialsId: 'docker-hub-credentials', usernameVariable: 'DOCKER_USERNAME', passwordVariable: 'DOCKER_PASSWORD')]) {
                        // Inside this block, DOCKER_USERNAME and DOCKER_PASSWORD are available
                        loginToDockerHub(DOCKER_USERNAME, DOCKER_PASSWORD)
                    }
                }
            }
        }
    }
}



