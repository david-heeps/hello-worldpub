pipeline {
    agent any
    stages {
        stage('Git Checkout') {
            steps {
                sh 'echo "Success!"'
            }
        }
      //  stage('Merging') {
      //      steps {
      //          sh 'echo "Merging test to Master!"'
    stage('CheckoutTest') {
        steps {
            git branch: 'master', url: 'ssh://git@github.com:david-heeps/hello-worldpub.git'
        }
    }
         //   }
     //   }
    }
}
