pipeline {
  agent any
  stages {
    stage('this_par') {
      parallel {
        stage('first') {
          steps {
            sh 'env'
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
