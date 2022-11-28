pipeline{
	agent any
	environment{
		staging_server="40.121.10.123"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r -v -o stricthostkeychecking=no ${WORKSPACE}/* jk-vm@${staging_server}:/var/www/html/'
			}
		}
	}
}
