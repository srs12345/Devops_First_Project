pipeline {
  agent {
    node {
      label 'Node 1'
    }

  }
  stages {
    stage('To Build image') {
      steps {
        sh 'docker build -t ubuntu:3.12.12.1 .'
      }
    }

  }
}