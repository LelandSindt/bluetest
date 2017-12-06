pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "Build"'
      }
    }
    stage('Deploy') {
      when {
        branch 'something-master'    //only run these steps on the master branch
      }
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
