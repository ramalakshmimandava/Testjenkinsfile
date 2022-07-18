pipeline{
    agent any
    environment{
        WORKSPACE = pwd()
    }
     parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
        string(name: 'Welcome', defaultvalue: 'Welcome to my Test', description: 'I welcome to all my location')
    }
  stages{
        stage('hai'){
          steps{
            echo "welcome to jenkins"
          }
        }
      stage('Parameter_Declaration') {
            steps {
                echo "${params.Greeting} World!"
                 echo "${params.Welcome} Namste!"
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
      stage("Env Variables"){
            steps{
                bat "set"                                                     
            }
        }
  }
    post {
        always {
            mail to: bhemanirao@gmail.com, subject: 'Iam testing jenkins:)'
            mail to: ramalakshmi.mandava@gmail.com, subject: 'Iam testing jenkins :)'
        }
        
    }
}
