pipeline {

    agent any  // This will run the pipeline on any available agent

    stages 
    {
        
        stage('Execute the test cases') 
        {
            steps
            {
                        bat "docker-compose up"
            }
        }

   stage('Bring down compose') 
        {
            steps
            {
                        bat "docker-compose up"
                    
            }
        }
    
    }
}
