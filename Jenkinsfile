pipeline {
    agent any
    stages {
       
        stage('Example') {
            steps {
                sh 'echo "Hello World"'
                sh 'echo "Hello World again710!!!"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
     }
        post {
        always {
            archiveArtifacts artifacts: 'bin/**/*.*', fingerprint: true
        }
    }
}
