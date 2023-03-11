pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        echo 'I BUILD'
      }
    }

    stage('TEST') {
      parallel {
        stage('TEST') {
          steps {
            echo 'I TEST'
          }
        }

        stage('DEPLOY') {
          steps {
            echo 'I DEPLOY'
          }
        }

      }
    }

  }
}