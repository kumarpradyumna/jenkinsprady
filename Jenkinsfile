pipeline{
 agent any
    stages{
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
           
            }
        }
    }
   
