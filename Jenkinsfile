pipeline{
	agent any

	stages{
		stage('Welcome'){
			steps{
				echo 'Starting jenkins Docker Pipeline!'
			      }
			      }
		stage('Build Docker Image'){
			steps{
				sh '''
				docker build -t  my-first-jenkins-image:1.0 .
				'''
				}
				}
		stage('Finish'){
			steps{
				echo 'Docker image built successfully!'
				}
				}
				}
				}
		
