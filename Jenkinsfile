pipeline {
    agent any
    stages {
        stage('Git Checkout') {
            steps {
                sh 'echo "Success!"'
            }
        }
        stage('Merging') {
            steps {
                sh 'echo "Merging test to Master!"'
                sh 'git checkout Master'
                sh 'git merge test'
            }
        }
    }
}
