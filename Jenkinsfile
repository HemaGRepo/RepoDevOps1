pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
      }
    }
    stage('Stage2') {
      steps {
        echo 'In Stage 2'
      }
    }
    stage('Test') {
      parallel {
        stage('Stage3') {
          steps {
            echo 'In Stage 3'
          }
        }
        stage('Integration test') {
          steps {
            echo 'Message 5'
          }
        }
      }
    }
  }
}