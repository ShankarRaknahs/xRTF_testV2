pipeline {
  agent any
  stages {
    stage('Preparation') {
      steps {
        sh 'ls'
        echo 'testing'
        sh '''cd ..
ls'''
      }
    }

    stage('Connection with TPF') {
      parallel {
        stage('Connection with TPF') {
          steps {
            sh '''ls
cd ..
ls'''
          }
        }

        stage('Connection with VP2') {
          steps {
            sh '''cd ..
ls'''
          }
        }

      }
    }

    stage('Validating the Data') {
      steps {
        sh 'ls'
      }
    }

    stage('Summary report generation') {
      parallel {
        stage('Summary report generation') {
          steps {
            sh 'ls'
          }
        }

        stage('test conf') {
          steps {
            readFile 'RTFCONF'
          }
        }

      }
    }

  }
}