pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            echo 'Build !'
            
          },
          "ping": {
            sh 'echo "salut"'
            
          }
        )
      }
    }
    stage('end') {
      steps {
        sh 'echo "ended"'
      }
    }
  }
}