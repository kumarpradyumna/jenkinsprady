pipeline {
    agent any 
    triggers {
        pollSCM ('*/1 * * * *')
    }
    options {
        timestamps()
        overrideIndexTriggers(false)
    }
    stages {
        stage ('checkout') {
            parallel {
                stage ('code')
            }
        }
        stage ('Build') {
         steps {
             echo 'Hello World 1 '
         }
        }
    }
}
