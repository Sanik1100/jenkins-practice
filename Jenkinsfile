pipeline{
	agent any
	stages{
		stage('Welcome'){
			steps{
				echo 'Hello from my Jenkinsfile!'
			}
			}
		stage('Build'){
			steps{
				sh '''
					echo "Building application..."
					mkdir -p app
					echo "hello from jenkinsfile" > app/message.txt
				'''
			}
			}
		stage('Test'){
			steps{
				sh '''
					echo "Testing application..."
					if [ -f app/message.txt ]; then
						echo "test passed!"
						cat app/message.txt
					else
						echo "test failed"
						exit 1
					fi
				'''
				}
				}
		stage('Finish'){
			steps{
				echo "Jenkinsfile execution completed"
				}
				}
				}
				}
