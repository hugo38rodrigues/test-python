pipeline {
	agent any
	stages {

		stage('Install depencies') {
			steps{
				script {
					sh 'python3 -m venv venv'
					sh '. venv/bin/activate'
					sh 'pip install -r requirements.txt'
		                 }
			}
	         }    
	}
}
