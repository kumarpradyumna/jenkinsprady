pipeline{
 agent any
    stages{
<<<<<<< HEAD
        stage("stages running in paralle"){
             paralle {
                 stage ("stage1") {
                     steps {
                         echo "1st stage executing"
                         sleep 2
                     }
                 }
                 stage ("stage2") {
                       steps {
                            echo "2nd stage executing"
                            sleep 2
                       }

                 }
                 stage ("stage3") {
                     steps {
                         echo "3rd stage executing"
                         sleep 2
                     }
                 }
                  

             }
=======
        stage("Build"){
<<<<<<< HEAD
            when {
                tag "release-*"
            }
=======
              when {
                  changelog(.*some_text.*)
              }
>>>>>>> b4a2d88... new line added
            steps{
                echo "Hello World Building tag"
            }
>>>>>>> 277dbcf... file added
           
            }
        }
    }
   
