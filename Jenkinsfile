pipeline {
  agent {
    node {
      label 'Node 2'
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