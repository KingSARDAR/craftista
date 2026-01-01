pipeline {
  agent any 
  tools {
    jdk 'JDK17'
    maven 'Maven'
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
