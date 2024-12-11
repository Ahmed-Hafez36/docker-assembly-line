pipeline {
  agent any

  stages {
    stage('Maven Check') {
      steps {
        bat 'mvn -version'
        bat 'java -version'
      }
    }
  }
}
