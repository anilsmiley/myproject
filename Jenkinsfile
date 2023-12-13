pipeline {
    agent any

    options {
        // Set the build discarder (logRotator) for this job
        buildDiscarder(logRotator(numToKeepStr: '30', artifactNumToKeepStr: '30'))
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from the repository
                echo "hello"
            }
        }

        stage('Build') {
            steps {
                // Build your Node.js and React application
                echo "boss"
            }
        }

        stage('Test') {
            steps {
                // Run tests (adjust this command based on your project)
                echo "great"
            }
        }

        stage('Deploy') {
            when {
                // Deploy only for the 'main' branch
                expression { currentBuild.branchName == 'main' }
            }
            steps {
                // Deploy to production (customize this step as needed)
                echo "code"
            }
        }
    }
}
