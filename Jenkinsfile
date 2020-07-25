pipeline{
    agent any
        stages{
        stage("Build"){
              when {
                  changerequest()
              }
            steps{
                echo "Hello world change request"
            }
           
        }
    }
}
  
