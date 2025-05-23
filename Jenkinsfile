pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                git branch: 'main', url: 'https://github.com/yassu974/seletores-cy.git'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'NO_COLOR=1 npm test'
            }
        }
    }
}