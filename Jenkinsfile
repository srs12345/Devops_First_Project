pipeline {
  agent {
    node {
      label 'Node 1'
    }

  }
  stages {
    stage('To access dockefile') {
      steps {
        sh 'cd /home/ubuntu/dockerp'
      }
    }

    stage('list the files') {
      steps {
        sh 'ls -la'
      }
    }

    stage('To build docker image') {
      steps {
        sh 'sudo docker build -t myjenkins-blueocean:2.401.3-1 .'
      }
    }

  }
}