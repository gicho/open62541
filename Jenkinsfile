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
            bat(script: 'eclipseheadless.bat', returnStatus: true, returnStdout: true)
            bat(script: 'bootblocker.bat', returnStatus: true, returnStdout: true)
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