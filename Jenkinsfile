
pipeline {
  agent any 
  stages {
    stage ('practice') {
      steps{
    script{
      def environments = [ "Development",
                           "QA",
                           "Production",
                           "DR"
                          ]
      for (environment in environments) {
         
        if (environment=="Production"){
          
        echo "environment reached-stopping deployment"
        echo "deploying to ${environment}" 
          break

        }
      }
    }
      }
    }
  }
}

    
