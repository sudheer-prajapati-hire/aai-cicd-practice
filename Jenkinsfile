pipeline {
    agent any

    stages {
        stage('1. Checkout Code') {
            steps {
                echo 'Fetching the latest code from repository...'
                // Real scenario mein yahan git checkout hota hai
            }
        }

        stage('2. Run Tests / Linting') {
            steps {
                echo 'Running code quality and syntax checks...'
                sh 'php -l index.php'
            }
        }

        stage('3. Build Docker Image (Simulated)') {
            steps {
                echo 'Building production Docker container image...'
                // sh 'docker build -t aai-app:latest .'
                echo 'Docker image built successfully!'
            }
        }

        stage('4. Deploy to Production Server') {
            steps {
                echo 'Deploying application containers to production environment...'
                echo 'Deployment Completed Successfully! 🚀'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully. Team notified!'
        }
        failure {
            echo 'Pipeline failed! Check logs immediately.'
        }
    }
}
