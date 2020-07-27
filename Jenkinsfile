pipeline {
    agent any 
    triggers {
        pollSCM ('*/1 * * * *')
    }
    options {
        timestamps()
        overrideIndexTriggers(true)
        buildDiscarder(logRotator (numToKeepstr: '5'))
       disableConcurrentBuilds()
    }
    stages {
        stage ('Build') {
         steps {
             echo 'Hello World 2 '
         }
        }
    }
} 
