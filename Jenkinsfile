pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh(
          label: "Delete all container",
          script: """
              docker-compose build
          """
        )
      }
    }
    stage('Run') {
      steps {
        sh(
          label: "Delete all container",
          script: """
              docker-compose up -d
          """
        )
      }
    }
    stage('Delete') {
      steps {
        sh(
          label: "Delete all container",
          script: """
              docker-compose down
          """
        )
      }
    }
  }
}
