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
        stage('Approval') {
            steps {
               script {
                echo "Approval Done"
               }
            }
        }

        stage('Deployment') {
            steps {
               script {
                properties([parameters([choice(choices: ['UAT','Stage'], description: 'Select Correct UCD environment', name: 'Environment1')])])
               }
            }
        }
    }
}
