pipeline{
    agent any
  stages{
        stage('hai'){
          steps{
            echo "welcome to jenkins"
          }
        }
      stage('filepath'){
          steps{
            //pomPath = findFiles(glob: "**/Simple.java")[0].path
           // env.WORKSPACE = pwd()
             echo pwd()  
                
          }
        }
          
        stage('Build') {
            steps {
                //dir("/var/lib/jenkins/workspace/demopipelinetask/my-app"){
                  sh 'javac Simple.java'
                //}
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
