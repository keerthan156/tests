pipeline{
	agent any
	environment{
		staging_server="20.121.122.115"
	}
	stages{
		stage('Deploy to remote'){
			steps{
				sh 'scp -p I$b6R!D1g2E02S1PymAA -r -P 22 ${WORKSPACE}/* ibllnxmetpyth@${staging_server}:/var/www/html/'
			}
		}
	}
}
