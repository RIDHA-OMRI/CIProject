pipeline {
    agent any
    
    tools {nodejs "node"}

    // Ridha Omri jenkins file
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build production files') {
            steps {
                sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                sh 'npm run test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'run deploy'
            }
        }
    }
}
