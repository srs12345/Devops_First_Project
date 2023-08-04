pipeline {
  agent {
    node {
      label 'Node 1'
    }

  }
  stages {
    stage('To access dockefile') {
      steps {
        sh 'cd /home/ubuntu/dockerf'
      }
    }

    stage('list the files') {
      steps {
        sh 'ls -la'
      }
    }

    stage('Builed an imag') {
      steps {
        sh '''sudo docker build . -t my-web-app -f /home/ubuntu/dockerf/Dockerfile
'''
      }
    }

  }
}