pipeline {
    agent none
    
    stages {
        stage('Angular Version') {
            steps {
                sh "ng version"
            }
        }
        
        stages {
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
