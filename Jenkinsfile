pipeline {
  agent any
  
  stages {
    stage('code checkin') {
      steps {
        git branch: 'main', url: 'https://github.com/sunithalakshmi/spring-petclinic.git'
      }
    }
    stage('code compile') {
      steps {
        sh 'mvn compile'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}
   
