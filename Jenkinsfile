pipeline {

  agent {
    label 'Linux'
  }
  
  stages {
    
    stage('Test') {
      
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
