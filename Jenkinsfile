pipeline{
	agent any
	environment{
		staging_server="20.121.122.115"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r -P 22 ${WORKSPACE}/* ibllnxmetpyth@${staging_server}:/var/www/html/'
			}
		}
	}
}
