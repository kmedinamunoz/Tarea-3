pipeline {
    agent none
    
    stages {
        stage('Angular Version') {
            steps {
                sh "ng version"
            }
        }
        
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

            stage('Install Dependencies') {
                steps {
                    sh "nmp install"
                }
            }
        }
    }
}
