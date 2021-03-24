pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Software'
      }
    }

    stage('Test') {
      parallel {
        stage('Test Windows') {
          steps {
            echo 'Windows'
          }
        }

        stage('Test Linux') {
          steps {
            echo 'Testing on Linux'
          }
        }

        stage('Test MacOS') {
          steps {
            echo 'Testing on MacOS'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment'
      }
    }

  }
}