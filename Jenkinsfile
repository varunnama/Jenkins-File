//@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script {
                input message:'Select environment for build', parameters: {choice(name:'Environment', choices: ['Build Only','Dev','Test'], description: 'Select Correct UCD environment')}
                //properties([parameters([choice(choices: ['Build Only','Dev','Test'], description: 'Select Correct UCD environment', name: 'Environment')])])]
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

    /*    stage('Deployment') {
            steps {
               script {
                input message:'Select UCD environment for deployment', parameters: [ 
                properties([parameters([choice(choices: ['UAT','Stage'], description: 'Select Correct UCD environment', name: 'Environment1')])])]
               }
            }
        }*/
    }
}
