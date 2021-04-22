pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
      sh '''#!/bin/bash          
    BUILD_TRIGGER_BY=$(curl -k --silent ${BUILD_URL}/api/xml | tr '<' '\n' | egrep '^userId>|^userName>' | sed 's/.*>//g' | sed -e '1s/$/ \//g' | tr '\n' ' ')
            echo "BUILD_TRIGGER_BY: ${BUILD_TRIGGER_BY}"
            }
          }
        }
     post { 
        always { 
            echo 'I will always say Hello again!'
        }
    }
}
