pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'First test  message...'
          }
        }
        stage('Build2') {
          steps {
            echo 'Print from Build2 step'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Test test'
      }
    }
  }
}