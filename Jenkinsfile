pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps{
                echo 'Checking out code...'
                git branch: 'main', url: 'https://github.com/Mithra07-Sriram/DEVOPS_CI.git'
            }
        }
        stage('Build Project') {
            steps {
                echo 'Building the project...'
                // For Windows commands use `bat` instead of `sh`
                bat 'echo Build successful'
            }
        }

        stage('Deploy Project') {
            steps {
                echo 'Deploying the project...'
                bat 'echo Deployment successful'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished execution.'
        }
        failure {
            echo '❌ Deployment failed!'
        }
    }
}
