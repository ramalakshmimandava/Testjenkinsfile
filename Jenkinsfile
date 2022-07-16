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
               
                 bat 'javac ${env.WORKSPACE}/Simple.java'
                
            }
        }
        stage('Run') {
            steps { 
                bat 'java ${env.WORKSPACE}/Simple'
                //java Simple
            }
        }
        
   
  }
}
