
pipeline {

    agent {
        node {
      label 'deploy'
    }

    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                // sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                l
                // sh 'npm test'
            }
        }
    }
}
