pipeline {
  agent any
  stages {
    stage('first') {
      agent {
        node {
          label 'any'
        }
        
      }
      environment {
        foo = 'bar'
      }
      steps {
        sh 'echo 42'
      }
    }
    stage('para') {
      parallel {
        stage('para') {
          agent {
            node {
              label 'any'
            }
            
          }
          steps {
            sh 'echo 43'
          }
        }
        stage('para2') {
          steps {
            sh 'echo 42'
          }
        }
      }
    }
  }
}