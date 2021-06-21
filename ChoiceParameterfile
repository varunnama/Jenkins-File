@Library('pipeline-library')

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
      
       stage('Deployment') {
            steps {
               script {
                
                echo "Deployment Completed For: $deploy_env"

                }
            }
        }
    }
}
