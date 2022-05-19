pipeline {
  agent any
  stages {
    stage('cloning') {
      steps {
        git(url: 'https://github.com/duongbm/eks-anywhere-gitops.git', branch: 'master')
      }
    }

    stage('error') {
      steps {
        script {
          commit = sh("git log -1 --pretty=%B")
          sh "echo $commit"
        }

      }
    }

  }
}