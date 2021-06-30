pipeline {
  agent any
  stages {
    stage('Poll code') {
      steps {
        git(url: 'git@code.ofweek.com:chenshunde/blade.git', branch: '"${BRANCH}"', changelog: true, credentialsId: 'dc2a13be-6348-4977-8772-7b59dd00a1fd')
      }
    }

  }
  environment {
    TAG = '""'
  }
}