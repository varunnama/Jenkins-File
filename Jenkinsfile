@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script {
                properties([parameters(choiceparameter.getBuildProperties())])
               }
            }
        }
    }
}