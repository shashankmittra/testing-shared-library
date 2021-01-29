pipeline{
	agent any

	stages{
		stage("clone"){
			steps{
				echo "Hello"
				scripts {
					def call(){
          					["git", "clone", "https://github.com/shashankmittra/simple-text.git"].execute()
					}
					call()
        				}		
				echo 'Branch - ' + env.GIT_BRANCH
				echo "done"
				echo "Workspace location: ${env.WORKSPACE}"
			}
		}
	}
}
