pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        echo '$PWD'
        archiveArtifacts artifacts: dist/trainSchedule.zip
      }
    }
  }
}
