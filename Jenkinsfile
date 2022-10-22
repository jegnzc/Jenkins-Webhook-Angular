pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        withSonarQubeEnv(installationName: 'SonarTest', credentialsId: 'jegnzc') {
          waitForQualityGate(abortPipeline: true, credentialsId: 'jegnzc', webhookSecretId: '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')
        }

      }
    }

  }
}