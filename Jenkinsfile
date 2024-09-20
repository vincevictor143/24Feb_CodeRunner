pipeline {

    agent any  // This will run the pipeline on any available agent

    stages {
        stage('Execute the test cases') {
            steps {
                script {
                    timeout(time: 20, unit: 'MINUTES') {
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
