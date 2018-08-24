pipeline {
  agent any
  stages {
    stage('Stage 0: Clone') {
      steps {
        git 'https://github.com/ZamElek/ProtectedData.git'
      }
    }
    stage('\'Stage 1: Clean\'') {
      steps {
        powershell(script: 'Invoke-Build Clean', returnStatus: true, returnStdout: true)
      }
    }
    stage('Stage 2: Analyze') {
      steps {
        powershell(script: 'Stage 3: Test', returnStatus: true, returnStdout: true)
      }
    }
  }
}