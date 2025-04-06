pipeline {
    agent any

    stages {
        stage('Clean') {
            steps {
                echo "Cleaning workspace..."
                sh "mvn clean"
            }
        }

        stage('Build') {
            steps {
                echo "Compiling..."
                sh "mvn compile"
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh "mvn test"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying..."
                // Add your deployment steps here
            }
        }
    }

    post {  // Optional, but helps in visualization
        always {
            echo "Pipeline completed!"
        }
    }
}
