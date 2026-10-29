pipeline{
  agent { label 'linux-agent' }

  stages {
    stage('Hello') {
      steps {
        echo 'Hello from my Linux Agent!'
      }
    }

    stage('System info') {
      steps {
        sh 'hostname'
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
