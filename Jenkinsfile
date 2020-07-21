pipeline {
  agent any
  stages {
    stage('Run on DEV') {
      parallel {
        stage('Run on DEV') {
          steps {
            bat 'echo "run on DEV"'
          }
        }

        stage('chrome') {
          steps {
            bat 'echo "run it on chrome"'
          }
        }

      }
    }

    stage('Run on QA') {
      parallel {
        stage('Run on QA') {
          steps {
            bat 'echo "run on QA"'
          }
        }

        stage('chrome') {
          steps {
            bat 'echo "run on chrome"'
          }
        }

        stage('firefox') {
          steps {
            bat 'echo "run on FF"'
          }
        }

      }
    }

    stage('Run on stage') {
      parallel {
        stage('Run on stage') {
          steps {
            bat 'echo "run on stage"'
          }
        }

        stage('chrome') {
          steps {
            bat 'echo "run on chrome"'
          }
        }

        stage('FF') {
          steps {
            bat 'echo "run on FF"'
          }
        }

        stage('stage') {
          steps {
            bat 'echo "run on safari"'
          }
        }

      }
    }

    stage('Run on PROD') {
      parallel {
        stage('Run on PROD') {
          steps {
            bat 'echo "run on prod"'
          }
        }

        stage('chrome') {
          steps {
            bat 'echo "run on chrome"'
          }
        }

      }
    }

  }
  tools {
    maven 'M3'
  }
}
