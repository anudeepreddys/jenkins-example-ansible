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
        docker { image 'alpine/ansible:latest' }
      }
      steps {
        sh 'ansible --version'
      }
    }
  }
}
