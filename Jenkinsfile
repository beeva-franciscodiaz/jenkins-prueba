#!groovy

pipeline {
    agent any

    stages {
        stage('First Stage') {
            steps {
                script{
            	    echo "Holaaaa"
                }
            }
        }
    }

    post {
        always {
            echo "We have been through the entire pipeline"
        }
        changed {
            echo "There have been some changes from the last build"
        }
        success {
            echo "Build successful"
        }
        failure {
            echo "There have been some errors"
        }
        unstable {
            echo "Unstable"
        }
        aborted {
            echo "Aborted"
        }
    }
}
