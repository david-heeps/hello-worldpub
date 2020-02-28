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
                sh 'git add -A'
                sh 'git commit -m "Merged test branch to master'
                sh 'git merge origin/test'
                sh 'git push origin HEAD:master'
            }
        }
    }
}
