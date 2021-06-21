@Library('pipeline-library')

def anything = 'nothing'

pipeline {
    agent any

    stages {

       stage('Build') {
            steps {
               script {
                def sel_val = properties([parameters(choiceparameter.getBuildProperties())])
               
                //echo "Selected Environment: ${sel_val}"
             
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
