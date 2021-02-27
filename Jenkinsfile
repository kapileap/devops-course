pipeline {
  agent any
  stages {
    stage('Test A') {
      agent {
        node {
          label 'Java8'
        }

      }
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

  }
  environment {
    BUZZ_NAME = 'Worker Bee'
  }
}