pipeline{
	agent any
	environment{
		staging_server="20.121.36.211"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r ${WORKSPACE}/* wuspythtlinprodAA@${staging_server}:/var/www/html/'
			}
		}
	}
}
