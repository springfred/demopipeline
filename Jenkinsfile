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
        stage('Test on Linux') {
          steps {
            echo 'Testing...'
          }
        }
        stage('Test on Windows') {
          steps {
            echo 'Test on Windows...'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying'
      }
    }
  }
}