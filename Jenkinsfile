
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
                    script {
                        switch(env.gitlabActionType) {
                            case 'PUSH':
                                echo "PUSH Event"
                                break
                            case 'MERGE':
                                echo "MERGE Event"
                                break
                            default:
                                echo "Default Value Event"
                        }
                    }
                }
        }
    }
}
