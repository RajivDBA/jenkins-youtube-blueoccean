pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test Steps'
          }
        }

        stage('Test per') {
          steps {
            echo 'Test Per'
          }
        }

      }
    }

    stage('Deploy / Print Message') {
      steps {
        echo 'Deply Print Message'
      }
    }

  }
}
