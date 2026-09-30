pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Install Dependencies') {
            steps {
                dir('frontend') {
                    bat 'npm install'
                }
            }
        }

        stage('Test') {
            steps {
                dir('frontend') {
                    bat 'npm test'
                }
            }
        }
    }
}