pipeline {
  agent any
  stages {
    stage('cloning') {
      steps {
        script {
          sh "git log -1 --pretty=%B"
        }

      }
    }

  }
}