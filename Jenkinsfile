// Importing global shared library
@Library('my-library') _

pipeline {
    agent any

    stages {
        stage('Docker Login') {
            steps {
                script {
                   DockerUtils.groovy()   
                }
            }
        }
    }
}




