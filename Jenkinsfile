pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh ""
               echo "Building Artifacts for project"
               
           }
       }
       stage('Reading branch wise')
       {
       when
       {
       branch "feature*"
       }
       steps
       {
       echo " It is only for Feature branch"
       }
       }

       stage('Deploy Code') {
	  

          steps {
               sh ""
               echo "Deploying Code"
               
          }
      }
      }
      }

