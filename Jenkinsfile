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
        stage ('Build') {
         steps {
             echo 'Hello World 2 '
         }
        }
    }
} 
