pipeline {
  agent any 

  
  stages {
    stage("one") {
      steps{
         echo 'compiling'
         sh 'mvn compile'
      }
    }

    stage ("two") {
      steps{
          echo 'testing'
          sh 'mvn clean test'
      }
    }

    stage("three") {
       steps {
         echo 'packaging'
         sh 'mvn package -DskipTests'
       }
    }
  }
}
