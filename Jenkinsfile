pipeline {
  agent { docker "maven" }

  stages {
    stage('maven') {
      steps {
        bat "mvn -version"
        bat "java -version"
      }
    }
  }
}
