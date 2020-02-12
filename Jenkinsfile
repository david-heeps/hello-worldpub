@Library('pipeline-library-demo') _

pipeline {
    agent any
    stages {
        stage('Example') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
