pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh(
          label: "Delete all container",
          script: """
              docker compose build --no-cache
          """
        )
      }
    }
  }
}
