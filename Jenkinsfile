pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building......'
      }
    }
    stage('Test firefox') {
      parallel {
        stage('Test firefox') {
          steps {
            sh 'echo \'Testing firefox\''
          }
        }
        stage('Testing Chrome') {
          steps {
            sh 'echo \'Testing chrome\''
          }
        }
        stage('Test safari') {
          steps {
            sh 'echo\'Testing safari\''
          }
        }
      }
    }
    stage('deploy') {
      steps {
        echo 'Deploying'
      }
    }
  }
}