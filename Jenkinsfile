pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
     BUILD_TRIGGER_BY = "${currentBuild.getBuildCauses()[0].shortDescription} / ${currentBuild.getBuildCauses()[0].userId}"
echo "BUILD_TRIGGER_BY: ${BUILD_TRIGGER_BY}""
            }
          }
        }
     post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
