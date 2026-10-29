pipeline{
  agent any

  stages {
    stage('Hello') {
      steps {
        echo 'Hello World from Jenkins Pipeline!'
      }
    }

    stage('System info') {
      steps {
        sh 'whoami'
        sh 'date'
      }
    }

    stage('Git Checkout') {
      steps {
        echo 'Pipeline completed successfully!'
      }
    }
  }
}
