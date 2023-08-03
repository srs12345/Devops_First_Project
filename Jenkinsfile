pipeline {
  agent {
    node {
      label 'Node 2'
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

    stage('To build docker image') {
      steps {
        sh 'docker build . -t myjenkins-blueocean:2.401.3-1 -f /home/ubuntu/dockerf/Dockerfile'
      }
    }

  }
}