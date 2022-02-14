pipeline {
  agent any
  stages {
    stage('Verify browsers are installed') {
      steps {
        sh 'google-chrome --version'
        sh 'firefox --version'
      }
    }
    stage('Running Tests') {
      steps {
        sh './mvnw clean test'
      }
    }
  }
}
