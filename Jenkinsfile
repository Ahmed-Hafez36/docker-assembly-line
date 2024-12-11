pipeline {
  agent any

  stages {
    stage('Maven Check') {
      steps {
        script {
          def workspacePath = pwd().replace('\\', '/').replace('C:', '/c')
          def mavenImage = docker.image('maven')
          mavenImage.inside("-v ${workspacePath}:/workspace -w /workspace") {
            bat "mvn -version"
            bat "java -version"
          }
        }
      }
    }
  }
}
