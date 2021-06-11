@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                properties([parameters(choiceparameter.getBuildProperties())])
            }
        }
    }
}