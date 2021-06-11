//@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script {
                properties([parameters([choice(choices: ['Build Only','Dev','Test'], description: 'Select Correct UCD environment', name: 'Environment')])])
               }
            }
        }
    }
}
