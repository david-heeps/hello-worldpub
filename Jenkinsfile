

properties([
    pipelineTriggers([
        [$class: "SCMTrigger", scmpoll_spec: "* * * * *"],
        ])
    ])

pipeline {
    agent any
    stages {
       
        stage('Example') {
            steps {
                sh 'echo "Hello World"'
                sh 'echo "Hello World again2!!!"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}
