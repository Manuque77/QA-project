pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Manuque77/QA-project'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}

