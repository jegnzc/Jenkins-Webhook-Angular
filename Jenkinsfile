pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        withSonarQubeEnv('SonarTest') {
          waitForQualityGate true
        }

      }
    }

  }
}