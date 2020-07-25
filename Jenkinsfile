pipeline {
    agent any 
    stages {
        stage ('Build master') {
            when {
                branch 'master'
            }
            steps {
                echo "Building master"
            }

        }
        stage ("Build sit") {
            when {
                branch 'sit'
            }
            steps {
                echo "Building sit"
            }
        }
          
          }
    }
}
