//@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script {
                input message:'Select environment for build', ok: 'Env!', parameters: [choice(name:'Environment', choices: ['Build Only','Dev','Test'], description: 'Select Correct UCD environment')]
                }
            }
        }
    }
}
