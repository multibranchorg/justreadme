pipeline {
  agent any
  stages {
    stage('Each of these takes ten seconds') {
      parallel {
        stage('first') {
          steps {
            echo 'First branch'
            script {
              sh 'for i in `seq 1 10`; do echo "Sleeping 1S"; sleep 1; done'
            }
            
          }
        }
        stage('second') {
          steps {
            echo 'Second branch'
            script {
              sh 'for i in `seq 1 10`;  do echo "Sleeping 1S"; sleep 1; done'
            }
            
          }
        }
      }
    }
  }
}