pipeline {
    agent any
    triggers { pollSCM('H */12 * * 1-5') }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
            }
        }
        stage('Stage Two') {
            steps {
                sh 'echo "hello stage 2"'
            }
        }
        stage('Stage Three') {
            steps {
                sh 'echo "hello stage 3"'
            }
        }
    }
}
