pipeline {
    agent any 
    triggers {
        pollSCM ('*/1 * * * *')
    }
    options {
        timestamps()
        overrideIndexTriggers(true)
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
