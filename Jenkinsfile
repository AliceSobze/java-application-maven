pipeline {
  agent any
  tools {
    maven "Maven1"
  }
  stages {
    stage ("maven clean") {
      steps {
       sh 'mvn clean' 
      }
    }
    stage ("maven package") {
      steps {
       sh 'mvn package' 
      }
    }
    stage ("docker build") {
      steps {
       sh 'docker build -t alicesobze2/jenkinsmaven .' 
      }
    }
    
  }
  
  
}
