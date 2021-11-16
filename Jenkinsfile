pipeline
{
	agent any
	 stages {
	  stage('Pull') {
		steps{
		   scripts{
  			checkout(([$class: 'GitSCM', branches: [[name: '*/master']],
				userRemotConfigs :[[
					url: 'https://github.com/hamzaabdelwahed9/hamzaCD.git' ]]])
			 }
		     }

          }
}
}						

