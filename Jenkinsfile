pipeline {

  agent {
    label 'Linux'
  }
  
  stages {
    
    stage('Test') {
      
      steps {
        sh 'mvn test'  
      }
      
    }
    
    stage('Publication') {
    
      steps {
        junit 'target/surefire-reports/*.xml'
      }
      
    }
    
  }
  
}
