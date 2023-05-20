pipeline{
	agent any
	stages{
		stage("Start Grid"){
			steps{
				sh 'docker-compose up chrome Firefox'
			}
		}
		stage("Bring Grid Down"){
			steps{
				sh 'docker-compose up search-module book-flight-module'
			}
		}
		stage("Bring Grid Down"){
			steps{
				sh 'docker-compose down'
			}
		}
	}
}