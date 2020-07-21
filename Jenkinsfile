pipeline {
  agent any
  stages {
    stage('Run on DEV') {
      parallel {
        stage('Run on DEV') {
          steps {
            sh 'echo "run on DEV"'
          }
        }

        stage('chrome') {
          steps {
            sh 'echo "run it on chrome"'
          }
        }

      }
    }

    stage('Run on QA') {
      parallel {
        stage('Run on QA') {
          steps {
            sh 'echo "run on QA"'
          }
        }

        stage('chrome') {
          steps {
            sh 'echo "run on chrome"'
          }
        }

        stage('firefox') {
          steps {
            sh 'echo "run on FF"'
          }
        }

      }
    }

    stage('Run on stage') {
      parallel {
        stage('Run on stage') {
          steps {
            sh 'echo "run on stage"'
          }
        }

        stage('chrome') {
          steps {
            sh 'echo "run on chrome"'
          }
        }

        stage('FF') {
          steps {
            sh 'echo "run on FF"'
          }
        }

        stage('stage') {
          steps {
            sh 'echo "run on safari"'
          }
        }

      }
    }

    stage('Run on PROD') {
      parallel {
        stage('Run on PROD') {
          steps {
            sh 'echo "run on prod"'
          }
        }

        stage('chrome') {
          steps {
            sh 'echo "run on chrome"'
          }
        }

      }
    }

  }
  tools {
    maven 'M3'
  }
}