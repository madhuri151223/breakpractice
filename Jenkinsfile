
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
        echo "deploying to ${environment}"
        if (environment=="Production"){
        echo "environment reached-stopping deployment"
          break

        }
      }
    }
      }
    }
  }
}

    
