pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh "mvn clean package"
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
       echo " It is only for Feature Branch"
       }
       }

       stage('Deploy Code') {
       when
       {
       branch "master"
       }
	  

          steps {
               sh "mvn tomcat7:deploy"
               echo "Deploying Code"
               
          }
      }
      }
      }

