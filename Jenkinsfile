pipeline {
  agent any

  environment {
    PATH = "${env.PATH};C:\\apache-maven-3.9.9-bin\\apache-maven-3.9.9\\bin"
  }

  stages {
    stage('Maven Check') {
      steps {
        bat 'mvn -version'
        bat 'java -version'
      }
    }
  }
}
