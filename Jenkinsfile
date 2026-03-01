pipeline {
  agent any

  tools {
    nodejs 'node18'
  }

  stages {
    stage('Build') {
      steps {
        sh '''
          node --version
          npm --version
          npm ci
          npm run build
        '''
      }
    }
  }
}