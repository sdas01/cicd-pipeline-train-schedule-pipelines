pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running automation build'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
        echo 'Build automation completed'
      }
    }
  }

}
