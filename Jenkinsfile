pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh ""
               echo "Building Artifacts for project"
               
           }
       }
       stage('Reading branch wise information')
       {
       when
       {
       branch "feature*"
       }
       steps
       {
       echo " It is only for Feature Branch"
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

