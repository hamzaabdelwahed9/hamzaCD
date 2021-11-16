pipeline
{
	agent any
	 stages {
	  stage('Pull') {
		steps{
		   script{
  			checkout([$class: 'GitSCM', branches: [[name: '*/master']],
				userRemoteConfigs :[[
					credentialsId: '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',
					url: 'https://github.com/hamzaabdelwahed9/hamzaCD.git' ]]])
						
		            }
		     } }
          stage('docker') {
             steps{
                script{
                    sh "ansible-playbook Ansible/docker.yml -i Ansible/inventory/host.yml "
                }
            }
        }

     }
}						

