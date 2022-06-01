//DECLARATIVE
pipeline {
	agent any
	stages{
		stage('Build') {
			steps{
				echo "Build"
			}
		}
		stage('Test') {
			steps{
				echo "Test"
			}
		}
		stage('Integration Test') {
			steps{
				echo "Integration Test"
			}
		}
	} 
	
	post{
		always{
			echo "Hello world Jenkins. Running always"
		}
		success{
			echo "This run when success"
		}
		Failure{
			echo "Running on Failure"
		}
	}
}