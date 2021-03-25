pipeline{
	agent any
	stages{

		stage("Start Grid"){
			steps{
				sh "docker-compose up -d hub chrome firefox"
			}
		}
		
		stage("Stop Grid"){
			steps{
				sh "docker-compose down"
			}
		}

		}
	}
		
		
		


