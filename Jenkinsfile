pipeline{
    agent any
  stages{
        stage('hai'){
          steps{
            echo "welcome to jenkins"
          }
        }
      
        stage('Build') {
            steps {
                  sh 'javac Simple.java'
               // javac Simple.java
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
