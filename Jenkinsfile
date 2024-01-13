pipeline {
    agent any  // Runs on any available agent (can be customized to a specific agent)

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the version control system (e.g., Git)
                git 'https://github.com/Sathesh119/Jenkins-Sonarqube-Docker.git'
            }
        }

       
    }

    post {
        success {
            // Actions to be taken if the pipeline succeeds
            echo 'Build and deployment succeeded!'
        }

        failure {
            // Actions to be taken if the pipeline fails
            echo 'Build or deployment failed. Please check logs for details.'
        }
    }
}
