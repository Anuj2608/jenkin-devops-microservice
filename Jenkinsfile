// Declarative Pipleline

pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				echo "Build"	
			}
		}
		stage('Test') {
			steps {
				echo "Test"	
			}
		}
		stage('Integration Test') {
			steps {
				echo "Integration Test"	
			}
		}
	} post {
		always {
			echo 'I like Jenkins!!'
		}
		success {
			echo 'I run when your successfull!'
		}
		failure {
			echo 'I run when your fail'
		}
	}
	
}
