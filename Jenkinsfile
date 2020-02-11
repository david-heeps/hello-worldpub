@Library('my-shared-library') _

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                sayHello 'Dave'
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
