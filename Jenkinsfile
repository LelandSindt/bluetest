pipeline {
    agent any
    triggers { pollSCM('H */12 * * 1-5') }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
            }
        }
        stage('Stage Three') {
            when {
                branch 'master'    //only run these steps on the master branch
            }
            steps {
                sh 'echo "hello stage 3"'
            }
            steps {
                input "Continue?"
            }
            steps {
                sh 'echo "woot"'
            }
        }
    }
}
