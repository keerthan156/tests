pipeline{
	agent any
	environment{
		staging_server="172.174.5.145"
		pass='I$b6R!D1g2E02P1E'
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -r -v -P 22 -o stricthostkeychecking=no ${WORKSPACE}/* ibllnxreps2admin@${staging_server}:/var/www/html/'
			}
		}
	}
}
