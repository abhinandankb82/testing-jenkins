pipeline 
{
    agent any

    stages 
	{
        stage('Build') 
		{
            steps 
			{
                echo 'Build Application'
            }
        }
		stage('Test') 
		{
            steps 
			{
                echo 'Test Application'
            }
        }
		stage('Deloy') 
		{
            steps 
			{
                echo 'Deploy Application'
            }
        }
    }
	
	post
	{
	    always
		{
		   emailext body: 'Status', subject: 'Jenkine_Pipeline_Handling_Failure', to: 'akb@csod.com'
		}
		
	} 
	
}
