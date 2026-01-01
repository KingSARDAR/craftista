pipeline {
  agent any
  stages {
    stage('Voting build') {
      steps {
        dir(path: 'voting') {
          sh 'mvn compile'
        }

      }
    }

    stage('') {
      steps {
        dir(path: '/voting') {
          sh 'mvn clean test'
        }

      }
    }

  }
  tools {
    jdk 'JDK17'
    maven 'Maven'
  }
  post {
    always {
      echo 'Pipeline completed successfully'
    }

  }
}