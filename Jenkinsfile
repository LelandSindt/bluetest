pipeline {
    agent any
    triggers { cron('H */4 * * 1-5') }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
            }
        }
    }
}
