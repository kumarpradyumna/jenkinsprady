pipeline{
    agent any
    stages {
        stage('Build') {
            when {
                Branch 'master'
            }
            steps {
                echo "Building master"
            }
            stage('Build sit') {
                when {
                    Branch 'sit'
                }
                steps{
                    echo "Buildig SIT"
                }
            }
        }
    }
}
