pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        input(message: 'continue?', id: '123', ok: 'ok')
      }
    }
  }
  triggers {
    pollSCM('H */12 * * 1-5')
  }
}