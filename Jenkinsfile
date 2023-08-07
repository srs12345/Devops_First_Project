pipeline {
  agent {
    node {
      label 'Node 1'
    }

  }
  stages {
    stage('Builed an imag') {
      steps {
        sh '''sudo docker build . -t my-web-app -f /home/ubuntu/dockerf/Dockerfile
'''
      }
    }

  }
}