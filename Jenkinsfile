pipeline {

agent any

     tools {
          maven 'maven'
     }

     stages{

          stage('Creation du jar ') {

               steps {
                         sh 'mvn clean install -DskipTests'
               }
			   
          }

          stage('build docker image sur serveur') {

               steps {
                         sh 'docker build -t ams_app_user12 .'
                    }
					

          }

		  
     }
}
