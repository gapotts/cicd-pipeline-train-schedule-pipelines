pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon -Dorg.gradle.java.home=/usr/local/opt/openjdk/bin'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
