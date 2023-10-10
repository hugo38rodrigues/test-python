pipeline {
    agent any
	stage('Install depencies') {
		steps{
			script {
				sh 'chmod -R 777 ./'
				sh'python3 -m venv venv'
				sh'source venv/bin/activate'
				sh'pip install -r requirements.txt'
	                 }
		}
         }    
}
