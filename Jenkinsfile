pipeline {
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
