pipeline{
	agent any
	stages{

		stage("Start Grid"){
			steps{
				sh "docker-compose up -d hub chrome firefox"
			}
		}
		stage("Run Test")
		{
			step{
				sh "docker-compose up search-module"
			}
		}
		stage("Stop Grid"){
			steps{
				sh "docker-compose down"
			}
		}

		}
	}
		
		
		


