pipeline {
    agent any 
    triggers {
        pollSCM ('*/1 * * * *')
    }
    options {
        timestamps()
        overrideIndexTriggers(true)
        buildDiscarder(logRotator (numToKeepStr: '5'))
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
