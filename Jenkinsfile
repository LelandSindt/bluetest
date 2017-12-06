pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        input(message: 'continue?')
        sh 'echo "continued"'
      }
    }
  }
  triggers {
    pollSCM('H */12 * * 1-5')
  }
}
