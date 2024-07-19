pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo "Running building automation"
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
