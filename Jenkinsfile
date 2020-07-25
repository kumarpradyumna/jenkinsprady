pipeline{
    agent any
    stages {
        stage('Build') {
            when {
                branch 'master'
            }
            steps {
                echo "Building master"
            }
            stage('Build sit') {
                when {
                    branch 'sit'
                }
                steps{
                    echo "Buildig SIT"
                }
            }
        }
    }
}
