pipeline {
  agent any
  stages {
    stage('Back-end') {
      steps {
        sh 'echo $USER'
      }
    }
    stage('Front-end') {
      agent {
        docker { image 'ansible:ubuntu1404' }
      }
      steps {
        sh 'ansible --version'
      }
    }
  }
}
