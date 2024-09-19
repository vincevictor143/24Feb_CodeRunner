pipeline
{
	stages
	{
		stage('Execute the test cases')
		{
			bat "docker-compose up"
		}

		stage('Teardown jenkins')
		{
			bat "docker-compose down"
		}

		
	}
}