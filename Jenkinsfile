pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        withSonarQubeEnv(installationName: 'test', credentialsId: 'jegnzc') {
          waitForQualityGate(abortPipeline: true, credentialsId: 'jegnzc', webhookSecretId: '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')
        }

      }
    }

  }
}
