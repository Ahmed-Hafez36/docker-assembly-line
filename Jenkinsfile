pipeline {
  agent none

  stages {

    stage('maven') {
      agent { docker "maven" }
      steps {
        bat "mvn -version"
        bat "java -version"
      }
    }

    stage('node') {
      agent { docker "node" }
      steps {
        bat "node --version"
      }
    }

    stage('python') {
      agent { docker "python" }
      steps {
        bat "python3 --version"
      }
    }

    stage('golang') {
      agent { docker "golang" }
      steps {
        bat "go version"
      }
    }

    stage('gradle') {
      agent { docker "gradle" }
      steps {
        bat "gradle --version"
      }
    }

  }
}
