pipeline {
  agent any
  
  stages {
    stage('code checkin') {
      steps {
        git branch: 'main', url: 'https://github.com/sunithalakshmi/spring-petclinic.git'
      }
    }
    stage('code build') {
      steps {
        sh 'mkdir test'
        sh 'cd test'
      }
    }
  }
}
   
