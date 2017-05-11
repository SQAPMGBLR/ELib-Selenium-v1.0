pipeline {
  agent any
  stages {
    stage('Checking out SCM') {
      steps {
        echo 'Checking out SCM'
        git(url: 'https://github.com/SQAPMGBLR/ELib-Selenium-v1.0', branch: 'master', credentialsId: 'sqapmgblr', poll: true)
      }
    }
    stage('Selenium Testing') {
      steps {
        bat 'selenium'
      }
    }
  }
}