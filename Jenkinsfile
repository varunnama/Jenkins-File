//@library('pipeline-library')

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               script {
                input message: 'Select Env for deploy', parameters: [choice(choices: ['UAT1', 'STAGE1'], description: 'Select correct env for deploy', name: 'Environment')]
                }
            }
        }
    }
}
