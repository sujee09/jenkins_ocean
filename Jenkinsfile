pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello!'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'python --version'
          }
        }

        stage('Test1') {
          steps {
            echo 'Hi!'
          }
        }

      }
    }

  }
}