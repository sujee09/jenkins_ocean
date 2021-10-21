pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello!'
        sh 'echo "Second step"'
        sleep 1
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

    stage('Deploy') {
      steps {
        echo 'Deploy!'
      }
    }

  }
}