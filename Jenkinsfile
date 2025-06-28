pipeline{
  agent any
  stages{
    stage('Checkout'){
      steps{
        echo 'cloning the repository....'
      }
    }
    stage('Build Docker Image'){
      steps{
        echo 'Building docker image....'
        sh 'docker build -t jenkins-web-2 .'
      }
    }
    stage('Run Docker container'){
      steps{
        ehco 'Running Docker container....'
        sh 'docker run -d -p 8082:80 
      }
    }
  }
}
