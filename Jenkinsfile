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
             stage('Copy Archive') {
                  steps {
                     script {
                 step ([$class: 'CopyArtifact',
                 projectName: 'Job2',
                 filter: "bin/**/*.*",
                 target: '../artifacts/Job2']);
             }
         }
     }
     }
        post {
        always {
            archiveArtifacts artifacts: 'bin/**/*.*', fingerprint: true
        }
    }
}
