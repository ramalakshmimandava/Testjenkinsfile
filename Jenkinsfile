pipeline{
    agent any
    environment{
        WORKSPACE = pwd()
    }
  stages{
        stage('hai'){
          steps{
            echo "welcome to jenkins"
          }
        }
      stage('filepath'){
          steps{
              echo "${env.WORKSPACE}"
                
          }
        }
          
     stage('Build') {
           steps {
               
                 bat 'javac Simple.java'
                
            }
        }
        stage('Run') {
            steps { 
                bat 'java Simple'
                //java Simple
            }
        }
        
   
  }
}
