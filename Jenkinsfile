pipeline {
  agent any
  stages {
    state('Build') {
      steps {
        sh 'echo "Build"'
      }
    }
    stage('Deploy') {
      steps {
        input(message: 'continue?')
        sh 'echo "continued"'
      }
    }
  }
  triggers {
    pollSCM('H */12 * * 1-5')
  }
}
