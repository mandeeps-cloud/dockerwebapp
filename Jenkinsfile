pipeline {
  environment {
    registry = "cloudzune/hello-kaniko"
    registryCredential = 'docker'
  }
  agent any
  stages {
    stage('Building image') {
      steps{
        script {
          docker.build registry + ":$BUILD_NUMBER"
        }
      }
    }
  }
}
