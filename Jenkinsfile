pipeline {
    agent any 

    options {
        timestamps()
        overrideIndexTriggers(true)
       buildDiscarder(logRotator(numToKeepStr: '5'))
       disableConcurrentBuilds()
    }
    stages {
        stage ('build') {
            steps{
                echo "Hello world 44444444444444444444444444444444444444444444"
            }
            
        }
    }
}
