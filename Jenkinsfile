pipeline { agent any

stages { stage('Checkout') { steps { checkout scm } }

stage('Check Python') { steps { bat '"C:\Users\user\AppData\Local\Python\bin\python.exe" --version' } }

stage('Test') { steps { bat '"C:\Users\user\AppData\Local\Python\bin\python.exe" -m pytest' } } } }