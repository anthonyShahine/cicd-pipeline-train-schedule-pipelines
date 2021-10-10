pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Start the building"
        sh './gradlew build  --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
