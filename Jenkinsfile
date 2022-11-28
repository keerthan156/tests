pipeline{
	agent any
	environment{
		staging_server="40.121.10.123"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r ${WORKSPACE}/* jk-vm@${staging_server}:/var/www/html/'
			}
		}
	}
}
