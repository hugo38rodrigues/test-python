pipeline {
    agent any
    
    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    // Build the Docker image using the Dockerfile
                    def customImage = docker.build('my-python-app')
                }
            }
        }
        
        stage('Run Docker Container') {
            steps {
                script {
                    // Run the Docker container
                    def customContainer = customImage.run("-p 8080:80")
                }
            }
        }
        
        stage('Execute Python Script') {
            steps {
                script {
                    // Execute your Python script inside the Docker container
                    sh 'docker exec -it my-python-app python script.py'
                }
            }
        }
    }
    
}
