pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo " hai how are you"'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'echo "entering into testing area"'
          }
        }
        stage('dbtest') {
          steps {
            sh 'echo "test db is running"'
          }
        }
        stage('chrome') {
          steps {
            sh 'echo " chrome"'
          }
        }
      }
    }
    stage('prod') {
      parallel {
        stage('prod') {
          steps {
            sh 'echo " fine dev"'
          }
        }
        stage('integration test') {
          steps {
            sh 'echo " do interation test"'
          }
        }
        stage('junit est') {
          steps {
            sh 'echo " junit is running"'
          }
        }
        stage('sanity ') {
          steps {
            sh 'echo " sanity is running "'
          }
        }
      }
    }
    stage('staging ') {
      steps {
        sh 'echo " staging ares is  voisible"'
      }
    }
    stage('production') {
      steps {
        sh 'echo " production is stage depoly is sucess"'
      }
    }
  }
}
