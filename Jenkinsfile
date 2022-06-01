//DECLARATIVE
pipeline {
	//agent any
	agent { 
		docker { image 'maven:3.8.5-jdk-11-slim'} 
	}
	stages{
		stage('Build') {
			steps{
				sh 'mvn --version'
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
		failure{
			echo "Running on Failure"
		}
	}
}