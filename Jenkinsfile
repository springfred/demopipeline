pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build...'
      }
    }
    stage('Test') {
      parallel {
        stage('Test on Window') {
          steps {
            echo 'Test on Windows'
          }
        }
        stage('Test on Linux') {
          steps {
            echo 'Test on Linux...'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy...'
      }
    }
  }
}