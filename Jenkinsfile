// Declarative Pipleline

pipeline {
	agent { docker { image 'node:13.8'} }
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				sh 'node --version'
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
	} 
	post {
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
