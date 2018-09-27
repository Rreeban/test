pipeline {
  
  agent {
    label 'Linux'
  }
  
  stages {
    
    stage('Test & Publication') {
      
      steps {
        sh 'mvn test'  
      }
      
      post {
        
        always {
          junit 'target/surefire-reports/*.xml'
        }
        
      }
      
    }
    
  }
  
}
