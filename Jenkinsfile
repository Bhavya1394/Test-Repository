pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to build this message'
      }
    }

    stage('Test') {
      steps {
        echo 'I want to test the message'
      }
    }

    stage('Stage') {
      parallel {
        stage('Stage') {
          steps {
            echo 'I want to stage this message'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy this message'
          }
        }

        stage('Operate') {
          steps {
            echo 'I want to operate this message'
          }
        }

      }
    }

  }
}