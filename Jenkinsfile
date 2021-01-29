pipeline{
	agent any

	stages{
		stage("clone"){
			steps{
				echo "Hello"
				git 'https://github.com/shashankmittra/simple-text.git'
				echo 'Branch - ' + env.GIT_BRANCH
				echo "done"
				echo "Workspace location: ${env.WORKSPACE}"
			}
		}
	}
}
