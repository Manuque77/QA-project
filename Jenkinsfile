pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch:'main', url: 'https://github.com/Manuque77/QA-project.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Run Cypress Tests') {
            steps {
                bat 'npx cypress run'
            }
        }
    }
}
