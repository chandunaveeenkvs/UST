pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo build'
      }
    }
    stage('Test') {
      parallel {
        stage('Unit') {
          steps {
            sh 'echo Unit'
          }
        }
        stage('Performance') {
          steps {
            sh 'echo performance'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo deploy'
      }
    }
  }
}