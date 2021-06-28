pipeline {
  agent any
  stages {
    stage('pull code') {
      steps {
        git(url: 'git@github.com:chenshunde0219/blade.git', branch: '"${BRANCH}"', changelog: true, credentialsId: 'dc2a13be-6348-4977-8772-7b59dd00a1fd')
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