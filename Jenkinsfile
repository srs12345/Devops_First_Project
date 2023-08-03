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

  }
}