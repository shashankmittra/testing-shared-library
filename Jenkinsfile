pipeline{
	agent any

	stages{
		stage("clone"){
			steps{
				echo "Hello"
				checkout([$class: 'GitSCM', userRemoteConfigs: [[url: 'http://git-server/shashankmittra/simple-text.git']]])
		
				echo 'Branch - ' + env.GIT_BRANCH
				echo "done"
				echo "Workspace location: ${env.WORKSPACE}"
			}
		}
	}
}
