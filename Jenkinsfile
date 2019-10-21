pipeline {
  agent any
  stages {
    stage('BUILD') {
      steps {
        sh 'echo BUILD'
      }
    }
    stage('MAVEN') {
      steps {
        sh 'echo MAVEN'
      }
    }
    stage('POST MAVEN') {
      parallel {
        stage('POST MAVEN') {
          steps {
            sh 'echo "POST MAVEN"'
          }
        }
        stage('Checkmarx') {
          steps {
            sh 'echo "Checkmark"'
          }
        }
      }
    }
    stage('DEPLOY') {
      steps {
        echo 'DEPLOY'
      }
    }
  }
}