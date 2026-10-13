pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Check Python') {
            steps {
                bat 'python --version'
            }
        }

        stage('Test') {
            steps {
                bat 'python -m unittest -v'
            }
        }
    }
}