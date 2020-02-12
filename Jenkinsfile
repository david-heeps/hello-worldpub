@Library('pipeline-library-demo') _

properties([
    pipelineTriggers([
        [$class: "SCMTrigger", scmpoll_spec: "* * * * *"],
        ])
    ])

pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
            git(
                poll: true
                    url: 'https://github.com/david-heeps/hello-worldpub',
                    branch: 'master'
                )
            git(
                poll: true
                    url: 'https://github.com/david-heeps/jenkins-test2',
                    branch: 'master'
                )
        }
    }
        
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
