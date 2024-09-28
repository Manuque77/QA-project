pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Manuque77/QA-project.git'
            }
        }
        stage('Install Dependencies') {
            steps {
                // Cambia al directorio de tu proyecto
                dir('NuevoProjectoQA') {
                    bat 'npm ci'
                }
            }
        }
        stage('Run Cypress Tests') {
            steps {
                // Cambia al directorio donde está cypress.config.js
                dir('NuevoProjectoQA') {
                    bat 'npx cypress run --config-file cypress.config.js'
                }
            }
        }
    }
}
