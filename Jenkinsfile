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
    stage('Create Artifact') {
      steps {
        sh 'echo "Jenkins assessment artifact" > assessment.txt'
        archiveArtifacts artifacts: 'assessment.txt', fingerprint: true
      }
    }
      
    stage('Git Checkout') {
      steps {
        echo 'Pipeline completed successfully!'
      }
    }
  }
}
