pipeline {
    agent any 
    triggers {
        pollSCM ('*/1 * * * *')
    }
    options {
        timestamp()
        overrideIndexTriggers(true)
    }
    stages {
        stage ('Build') {
         steps {
             echo 'Hello World 1 '
         }
        }
    }
} 
