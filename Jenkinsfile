pipeline {
    agent any
    triggers { pollSCM('H */12 * * 1-5') }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
            }
        }
    }
}
