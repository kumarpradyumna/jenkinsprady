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
                stage ('code') {
                    steps{
                        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/kumarpradyumna/jenkinsprady.git']]])
                    }
                }
            }
        }
        stage ('Build') {
         steps {
             echo 'Hello World 1 '
         }
        }

    }
            defchangelogFound = false
def changeLogSets = currentBuild.changeSets
println "changeLogSets.size(): ${changeLogSets.size()}"
for (int i=0; changeLogSets.size(); i++) {
    println changeLogSets[i].getClass().getName()
    def entries = changeLogSets[i].items
    for (int j =0; j< entries.length; j++) {
        def entry = entries [j]
        println "${entry.msg}"
        if (entry.msg == /.*some_test.*) {
            changeLogFound = true
            break;
        }
    }

    if(changeLogFound)
    break
}
}
