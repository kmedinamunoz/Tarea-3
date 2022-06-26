pipeline {
    agent any
    
    stages {
        stage('Angular Version') {
            steps {
                sh "ng version"
            }
        }
        
        stage('Versions') {
            steps {
                sh 'node --version'
                sh 'npm --version'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh "npm install"
            }
        }
    }
}
