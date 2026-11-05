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
				docker build -t  my-first-jenkins-image:$BUILD_NUMBER .
				'''
				}
				}
		stage('Test Docker Image'){
			steps{
				sh '''
				echo "Testing Docker image..."
				docker run --rm my-first-jenkins-image:$BUILD_NUMBER
				'''
				}
				}
		stage('Finish'){
			steps{
				echo 'Docker image built and test successfully!'
				}
				}
				}
				}
		
