pipeline {
  agent {
    docker {
      args '-v /Users/arashid/.m2'
      image 'maven:3.5.2-jdk-8:/'
    }
    
  }
  stages {
    stage('initialize') {
      steps {
        sh '''echo PATH = ${PATH}
echo M2_HOME = ${M2_HOME}
mvn clean'''
      }
    }
  }
}