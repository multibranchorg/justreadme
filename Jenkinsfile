pipeline {
  agent any
  stages {
    stage('this_par') {
      parallel {
        stage('first') {
          steps {
            sh '''ls -lah
'''
          }
        }
        stage('second') {
          steps {
            sh 'ls -lah'
          }
        }
      }
    }
  }
}