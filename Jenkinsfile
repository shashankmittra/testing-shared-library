pipeline{
	agent any

	stages{
		stage("clone"){
			steps{
				echo "Hello"
				checkout([$class: 'GitSCM', branches: [[name: '*/master']] userRemoteConfigs: [[url: 'https://github.com/shashankmittra/simple-text.git']]])
		
				echo 'Branch - ' + env.GIT_BRANCH
				echo "done"
				echo "Workspace location: ${env.WORKSPACE}"
			}
		}
	}
}
