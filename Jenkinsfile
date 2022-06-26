pipeline {
    agent any
    
    stages {
        stage('Angular Version') {
            steps {
                sh 'ng version'
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
                sh 'npm install'
            }
        }

        stage('Lint Test Execution') {
            steps {
                sh 'npm run lint'
            }
        }

        // stage('Unit Test Execution') {
        //     steps {
        //         sh 'npm run test'
        //     }
        // }

        // stage('Sonar Execution') {
        //     steps {
        //         withSonarQubeEnv('sq-1'){
        //             sh 'npm run sonar'
        //         }
        //     }
        // }

        // stage('Quality Gate Validation') {
        //     steps {
        //         waitForQualityGate abortPipeline: true
        //     }
        // }

        // stage('Build Execution') {
        //     steps {
        //         sh 'npm run build'
        //     }
        // }
        
        // stage('Deploy Application') {
        //     steps {
        //         sh 'cp dist/tarea-3/* /var/www/html'
        //     }
        // }
    }
}