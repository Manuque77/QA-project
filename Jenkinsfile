pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Manuque77/QA-project.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Run Cypress Tests') {
            steps {
                sh 'npx cypress run'
            }
        }
    }
}
