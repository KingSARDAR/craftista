pipeline {
  agent any 
  tools {
    maven 'Maven 3.9.6'
  }
  stages {
   stage('Voting build') {
     steps {
       dir('voting') {
	sh 'mvn compile'
      }
     }  
   }
 }
 post {
  always {
   echo 'Pipeline completed successfully'
  }
 } 
}
