pipeline {
  agent any
  stages {
    stage ('Build') {
      step {
        echo 'Running build automation'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      } 
    }
  }
}
