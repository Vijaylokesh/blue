pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo %name%'
          }
        }
        stage('DB unit') {
          steps {
            sh 'echo hai'
          }
        }
        stage('jasmine') {
          steps {
            bat(returnStdout: true, script: 'echo %name%')
          }
        }
      }
    }
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sh 'echo $shell'
          }
        }
        stage('Edge') {
          steps {
            echo 'hai how are you'
          }
        }
        stage('safari') {
          steps {
            sh 'echo " do well"'
          }
        }
        stage('chrome') {
          steps {
            sh 'echo " my name is devil"'
          }
        }
      }
    }
    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'enter to dev'
          }
        }
        stage('bvt') {
          steps {
            sh 'echo " test cases run suceesfully"'
          }
        }
      }
    }
    stage('Staging ') {
      steps {
        sh 'echo " enter to staging area"'
      }
    }
    stage('production') {
      steps {
        echo 'finally we deployed'
      }
    }
  }
}