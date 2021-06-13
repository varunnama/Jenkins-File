@library('pipeline-library')

pipeline {
    agent any

    stages {

       stage('Arifact upload to Nexus') {
            steps {
               script {
                def fun_return = choiceparameter.getBuildProperties()
                echo "Nexus upload is completed"
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
