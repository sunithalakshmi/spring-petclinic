pipeline {
  label 'suni'
  
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
    stage('code test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('code build') {
      steps {
        sh 'mvn package'
      }
    }
    stage('code deploy') {
      steps {
        sh 'java -jar /home/ubuntu/workspace/pipeline/target/spring-petclinic-2.7.3.jar'
      }
    }
  }
}
   
