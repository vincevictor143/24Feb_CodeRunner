pipeline {
<<<<<<< HEAD
    stages {
        stage('Execute the test cases') {
            steps {
                script {
                    timeout(time: 10, unit: 'MINUTES') {
                        bat "docker-compose up"
                    }
                }
            }
        }
    }
    post {
        always {
            bat "docker-compose down"
        }
    }
}
=======
    agent any  // Define where to run the pipeline

    stages {
        stage('Execute the test cases') {
            steps {
                bat "docker-compose up"
            }
        }

        stage('Teardown jenkins') {
            steps {
                bat "docker-compose down"
            }
        }
    }
}
>>>>>>> 41ad77b1f00c1a9cd9290863663fbe643013bf37
