@Library('pipeline-library')

def anything = 'nothing'
def deploy_env= params.Environment

pipeline {
    agent any

    stages {

       stage('Build') {
            steps {
               script {
                properties([parameters(choiceparameter.getBuildProperties())])
               
                echo "Selected Environment: ${deploy_env}"
             
                }
            }
        }
      /*  stage('Deployment') {
            steps {
               script {
                def input_msg = input message: 'Select Env for deploy', parameters: [choice(choices: ['UAT', 'STAGE'], description: 'Select correct env for deploy', name: 'Environment')]
                echo "Selected Deployment Environment: $input_msg"
                }
            }
        }*/
    }
}
