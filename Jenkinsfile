pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                echo 'Cloning the remote repository...'
                // Replace with your Git repository URL
                git branch: 'main', url: 'https://github.com/ram-maker/Jenkins_test.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Running build steps...'
                // Example: Run a shell script from the cloned repository
                sh 'echo "Hello from the pulled repository!"'
            }
        }
    }
    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the logs for details.'
        }
    }
}

