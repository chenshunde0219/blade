pipeline {
  agent any
  stages {
    stage('pull code') {
      steps {
        git(url: 'https://github.com/chenshunde0219/blade.git', branch: '"${BRANCH}"', changelog: true, credentialsId: 'GIT_USER')
      }
    }

    stage('print') {
      steps {
        sh '''sh """
  ls
"""'''
      }
    }

  }
  environment {
    TAG = '""'
  }
}