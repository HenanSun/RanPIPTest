pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "test"'
          }
        }
        stage('test') {
          steps {
            sh 'echo "1"'
          }
        }
      }
    }
    stage('deliver') {
      steps {
        input 'Finished using the web site? (Click "Proceed" to continue)'
      }
    }
  }
}