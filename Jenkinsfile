pipeline{
    agent any
  stages{
    stage('hai'){
      steps{
        echo "welcome to jenkins"
      }
    }
      stages {
        stage('Build') {
            steps {
                javac Simple.java
            }
        }
        stage('Run') {
            steps {
                java Simple
            }
        }
    }
  }
}
