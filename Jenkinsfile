pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                dir('nutriflow/frontend') {
                    bat 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                dir('nutriflow/frontend') {
                    bat 'npm test'
                }
            }
        }
    }
}