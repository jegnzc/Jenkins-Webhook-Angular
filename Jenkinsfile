pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        withSonarQubeEnv(installationName: 'sonar-scanner', credentialsId: 'jegnzc') {
          waitForQualityGate(abortPipeline: true, credentialsId: 'jegnzc', webhookSecretId: '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')
        }

      }
    }

  }
}
