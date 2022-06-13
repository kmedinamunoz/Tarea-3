pipeline {
    agent { dockerfile true
        // dockerfile {
        //     image ''
        //     args '--mount type=volume,src=jenkins_tarea3,dst=/tmp'
        // }
    }

    stages {
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Unit Test') {
            steps {
                echo 'Ejecutando Unit Test'
            }
        }

//         stage('Sonar Scanner') {
//             steps {
//                 sh 'npm run sonar'
//             }
//         }

        stage('Build Application') {
            steps {
                sh 'npm run build'
            }
        }
      
        stage('Deploy Application') {
            steps {
                sh 'cp dist/tarea3/* /tmp/'
            }
        }
    }
}