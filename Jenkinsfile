pipeline {
  agent any
  stages {
    stage('Test A') {
      agent any
      steps {
        echo 'Bees Buzz'
        stash(name: 'Buzz TestA', includes: 'target/**')
      }
    }

    stage('Bees Bees') {
      steps {
        echo 'Buzz, Bees, Buzz!'
        echo 'Bees Buzzing!'
      }
    }

    stage('Confirm Deploy to Staging') {
      steps {
        input(message: 'Do you want to deploy to staging?', ok: 'lets do it!')
      }
    }

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}