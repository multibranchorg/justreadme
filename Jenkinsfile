pipeline {
  agent any
  stages {
    stage('thing') {
      agent {
        node {
          label 'foo'
        }
        
      }
      steps {
        sh 'echo 42244'
      }
    }
    stage('fdsfds') {
      parallel {
        stage('fdsfds') {
          agent any
          environment {
            foo = 'bar'
          }
          steps {
            sh 'echo 423'
          }
        }
        stage('fdsafsda') {
          steps {
            sh 'echo 42'
          }
        }
      }
    }
  }
}