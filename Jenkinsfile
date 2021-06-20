@Library('pipeline-library')

pipeline {
    agent any

    stages {

       stage('Arifact upload to Nexus') {
            steps {
               script {
               // def fun_return = choiceparameter.getBuildProperties()
                //echo "Parameter: ${fun_return}"
                choiceparameter.call('Varun Nama')
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
