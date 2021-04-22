pipeline {
    agent any
    stages {
        stage('preparation') {
            steps {
                script{
                    def buildCause = currentBuild.getBuildCause()[0].shortDescription
                    echo " Current build was caused by: ${buildCause}\n"
                }
            }
        }
    }
}
               
