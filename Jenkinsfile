pipeline{
	agent any
	environment{
		staging_server="168.61.51.87"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r ${WORKSPACE}/* ibllnxreps2admin@${staging_server}:/var/www/html/'
			}
		}
	}
}
