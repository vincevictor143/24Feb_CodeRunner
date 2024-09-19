pipeline {
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
