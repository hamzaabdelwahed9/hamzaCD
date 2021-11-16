pipeline
{
	agent any
	 stages {
	  stage('Pull') {
		steps{
		   scripts{
  			checkout(([$class: 'GitSCM', branches: [[name: '*/master']],
				userRemoteConfigs :[[
					credentialsId: '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',
					url: 'https://github.com/hamzaabdelwahed9/hamzaCD.git' ]]])
						
		            }
		     }

          }

     }
}						

