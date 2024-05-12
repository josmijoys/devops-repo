pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                // Check out the code from the Git repository
                git 'https://github.com/josmijoys/devops-repo.git'
            }
        }
        stage('Build') {
            steps {
                // Execute build steps, such as compiling code or running tests
                sh 'echo /var/lib/jenkins/workspace/devops_assignment/directory2/hello.sh' // Example Maven build command
            }
        }
        // Add more stages as needed
    }
    
    post {
        success {
            // Send a notification or perform additional actions on successful build
            echo 'Pipeline execution completed successfully!'
        }
        failure {
            // Send a notification or perform additional actions on failed build
            echo 'Pipeline execution failed!'
        }
    }
}
