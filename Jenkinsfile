pipeline {
    agent any
    triggers { cron('H */12 * * 1-5') }
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
    }
}
