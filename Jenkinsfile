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
                bat 'npm ci'
            }
        }
        stage('Run Cypress Tests') {
            steps {
                dir('NuevoProjectoQA') {
                    bat 'dir'  // Verifica la estructura de archivos
                    bat 'npx cypress run --config-file cypress.config.js'
                }
            }
        }
    }
}
