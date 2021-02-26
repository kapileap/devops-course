pipeline {
  agent any
  stages {
    stage('Buzz Buzz') {
      steps {
        echo 'Bees Buzz'
        sh 'echo "I am a ${BUZZ_NAME}"'
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