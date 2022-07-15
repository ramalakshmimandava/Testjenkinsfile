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
               
                  sh 'javac ${env.WORKSPACE}/Simple.java'
                
            }
        }
        stage('Run') {
            steps { 
                sh 'javac Simple'
                //java Simple
            }
        }
   
  }
}
