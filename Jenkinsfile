pipeline {
  agent any
  stages {
    stage('cloning') {
      steps {
        git(url: 'https://github.com/duongbm/eks-anywhere-gitops.git', branch: 'master')
        script {
          sh(returnStdout: true, script: 'git log -1 --pretty=%B')
        }

      }
    }

  }
}