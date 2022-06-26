pipeline {
    agent none
    
    stages {
        agent {
                docker { image 'node:16.15.1-alpine' }
            }
        stage('Versions') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }
    }
}
