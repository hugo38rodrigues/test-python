pipeline {
    agent any
    
    }
    
    post {
        always {
            // Clean up by stopping and removing the container
            script {
                customContainer.stop()
                customContainer.remove()
            }
        }
    }
}
