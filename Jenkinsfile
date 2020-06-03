pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'Running build automaion'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
