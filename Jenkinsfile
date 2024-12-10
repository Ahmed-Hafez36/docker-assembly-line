pipeline {
  agent any

  stages {
    stage('Maven Check') {
      steps {
        script {
          // Ensure Docker runs the Maven image with appropriate volumes mapped
          def mavenImage = docker.image('maven')
          mavenImage.inside('-v ${pwd()}:/workspace -w /workspace') {
            sh "mvn -version"
            sh "java -version"
          }
        }
      }
    }
  }
}
