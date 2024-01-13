pipeline {
    agent agent  // Runs on any available agent (can be customized to a specific agent)

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the version control system (e.g., Git)
                git 'https://github.com/Sathesh119/Jenkins-Sonarqube-Docker.git'
            }
        }

        stage('Build') {
            steps {
                // Build the project (replace with your build tool and commands)
                sh 'mvn clean install'  // Example for Maven build
            }
        }

        stage('Test') {
            steps {
                // Run tests (replace with your testing commands)
                sh 'mvn test'  // Example for Maven test
            }
        }

        stage('Deploy') {
            steps {
                // Deployment steps (replace with your deployment commands)
                sh 'echo "Deploying to production"'  // Example deployment command
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
