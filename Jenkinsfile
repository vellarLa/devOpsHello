pipeline {

  environment {
    dockerimagename = "vallarla/hello"
    dockerImage = ""
  }

  agent any

  stages {

    stage('Checkout Source') {
      steps {
        git 'https://github.com/vellarLa/devOpsHello'
      }
    }

    stage('Build image') {
      steps {
        git 'https://github.com/vellarLa/devOpsHello'
      }
    }

    stage('Pushing Image') {
      environment {
               registryCredential = 'dockerhub-credentials'
           }
      steps{
         git 'https://github.com/vellarLa/devOpsHello'
        }
      }
    }

    stage('Deploying container to Kubernetes') {
      steps {
         git 'https://github.com/vellarLa/devOpsHello'
      }
    }

  }

}
