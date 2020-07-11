pipeline {
  agent any
  stages {
    stage('1stage') {
      steps {
        sh 'echo "1st display"'
      }
    }

    stage('2stage') {
      parallel {
        stage('2stage') {
          steps {
            sh 'echo "2nd stage dispalay"'
          }
        }

        stage('3 stage') {
          steps {
            echo 'Hi i am 3ed stage'
          }
        }

      }
    }

  }
}