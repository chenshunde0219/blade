pipeline {
  agent any
  stages {
    stage('Poll code') {
      steps {
        git(url: 'https://github.com/chenshunde0219/blade.git', branch: 'master', changelog: true)
      }
    }

  }
  environment {
    TAG = '""'
  }
}