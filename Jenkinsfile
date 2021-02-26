pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      parallel {
        stage('Test A') {
          steps {
            echo 'Bees Buzz'
            sh 'echo "I am a ${BUZZ_NAME}"'
          }
        }

        stage('TestB') {
          steps {
            sh '''sleep 10
echo done.'''
          }
        }

      }
    }

    stage('Bees Bees') {
      steps {
        echo 'Buzz, Bees, Buzz!'
        echo 'Bees Buzzing!'
      }
    }

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}