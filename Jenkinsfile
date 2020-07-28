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
        stage ('build') {
            echo "Hello world 1"
        }
    }
}}
