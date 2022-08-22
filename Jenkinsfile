pipeline{
    agent any
    environment{
        WORKSPACE = pwd()
    }
    // triggers {
        //cron('*/2 * * * *')
        //  cron('H */4 * * 1-5')
   // }
    //adding parameters (18/7/2022)
     parameters {
        string(name: 'Greeting', defaultValue: 'Hello', description: 'How should I greet the world?')
        string(name: 'Welcome', defaultValue: 'Welcome to my Test', description: 'I welcome to all my location')
    }
  stages{
        stage('hai'){
          steps{
            echo "welcome to jenkins"
          }
        }
       //adding Parameter_Declaration stage (18/7/2022)
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
      //adding Env Variables stage (18/7/2022)
//       stage("Env Variables"){
//             steps{
//                 bat "set"                                                     
//             }
//         }
     /*  stage('Artifacts'){
            steps{
                echo "Hello World!" %WORKSPACE%/buildArtifact.txt
               }
        }*/
  }    
     //adding post build action (18/7/2022)
    post {
        always {
            echo 'thank you'
           // mail to: bhemanirao@gmail.com, subject: 'Iam testing jenkins:)'
           //mail to: ramalakshmi.mandava@gmail.com, subject: 'Iam testing jenkins :)'
        }
    }
}
