// Importing global shared library
@Library('my-library') _

pipeline {
    agent any

    stages {
        stage('Docker Login') {
            steps {
                // Call the loginToDockerHub method from the imported library
                DockerUtils.loginToDockerHub()
            }
        }
    }
}



