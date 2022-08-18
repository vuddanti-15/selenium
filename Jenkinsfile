pipeline {
  agent any
  stages {
    stage('Verify browsers are installed') {
      steps {
        sh 'google-chrome --version'
        sh 'firefox --version'
      }
    }
    stage('Run Tests') {
      steps {
        sh 'mvn clean install'
        sh 'mvn clean test'
      }
    }
  }
}
