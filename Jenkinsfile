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
                sh 'git fetch master'
                sh 'git checkout master'
                sh 'git merge test'
            }
        }
    }
}
