pipeline{
	agent any

	stages{
		stage("clone"){
			steps{
				echo "Hello"
				dir('cloned'){
				checkout([$class: 'GitSCM', branches: [[name: '*/main']], userRemoteConfigs: [[url: 'https://github.com/shashankmittra/simple-text.git']]])
				}
				echo 'Branch - ' + env.GIT_BRANCH
				echo "done"
				echo "Workspace location: ${env.WORKSPACE}"
			}
		}
	}
}
