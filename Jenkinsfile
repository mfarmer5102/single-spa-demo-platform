pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo 'Hello world!'
      }
    }

    stage('Build') {
      steps {
        sh 'docker build -t myapp:latest .'
      }
    }

    stage('Run Locally') {
      steps {
        sh 'docker run myapp:latest'
      }
    }

  }
}