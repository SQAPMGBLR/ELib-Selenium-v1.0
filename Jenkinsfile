pipeline {
  agent any
  stages {
    stage('Checking out SCM') {
      steps {
        echo 'Checking out SCM'
        git(url: 'https://github.com/SQAPMGBLR/ELib-Selenium-v1.0', branch: 'master', credentialsId: 'sqapmgblr', poll: true)
      }
    }
    stage('Sonarqube Analysis') {
      steps {
        echo 'SonarQube analysis started .....'
        bat 'sonar-scanner'
        echo 'SonarQube analysis completed successfully .....'
      }
    }
    stage('Launch Sonarqube') {
      steps {
        bat 'Sonar'
      }
    }
    stage('Selenium Testing') {
      steps {
        bat 'selenium'
        echo 'Selenium script is completed'
      }
    }
  }
}