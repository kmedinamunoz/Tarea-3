pipeline {
    agent any
  
    stages {
        stage('Angular Verification') {
            steps {
                sh "ng version"
            }
        }
        
        
        stage('Node Steps') {
            agent {
                docker { image 'node:16.13.1-alpine' }
            }
            stages{
                stage('Dependencies Installation') {
                    steps {
                        sh "npm install"
                    }
                }
            }
        }

    //     stage('Lint Test Execution') {
    //         steps {
    //             sh "npm run lint"
    //         }
    //     }

    //     stage('Unit Test Execution') {
    //         steps {
    //             sh "npm run test"
    //         }
    //     }

    //     stage('Sonar Execution') {
    //         steps {
    //             withSonarQubeEnv('sq-1'){
    //                 sh "npm run sonar"
    //             }
    //         }
    //     }

    //     stage('Quality Gate Validation') {
    //         steps {
    //             waitForQualityGate abortPipeline: true
    //         }
    //     }

    //     stage('Build Execution') {
    //         steps {
    //             sh "npm run build"
    //         }
    //     }
        
    //     stage('Deploy Application') {
    //         steps {
    //             sh "cp dist/tarea-3/* /var/www/html"
    //         }
    //     }
    }

    post {
        always {
            cleanWs()
        }
    }
}
