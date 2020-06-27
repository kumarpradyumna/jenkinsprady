pipeline {
    agent any
	
	stages {
        stage ('SCM') {
            steps {
                 git 'https://github.com/kumarpradyumna/java-tomcat-maven-example.git'
            }
		}
    
	    stage ('Build') {
            steps {
                 sh label: '', script: 'mvn package'
            }
		}
		
		stage ('archival') {
		  steps {
		     archive 'target/*.war'
			 }
		  
		}
    }
}

