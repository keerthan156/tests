pipeline{
	agent any
	environment{
		staging_server="172.174.5.145"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r -v -o stricthostkeychecking=no ${WORKSPACE}/* ibllnxreps2admin@${staging_server}:/var/www/html/'
			}
		}
	}
}
