pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        parallel(
          "build": {
            echo 'Build !'
            echo 'Nouvelle Task'
            
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