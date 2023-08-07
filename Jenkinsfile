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

    stage('Renaming the image') {
      steps {
        sh 'sudo docker tag my-web-app srs12345/devops-first-proj:v1'
      }
    }

    stage('Login to the docker hub') {
      environment {
        DOCKERHUB_USER = 'srs12345'
        DOCKERHUB_PASSWORD = 'Welcome@123'
      }
      steps {
        sh 'sudo docker login -u $DOCKERHUB_USER -p $DOCKERHUB_PASSWORD'
      }
    }

  }
}