pipeline { agent any

    stages { 
        stage('Example') {
            steps {
                bat 'echo Hello'
            }
        }
        stage('Checkout') { steps { checkout scm } }

        stage('Check Python') { steps { bat '"C:/Users/user/AppData/Local/Python/bin/python.exe" --version' } }

        stage('Install Dependencies') { steps { bat '"C:/Users/user/AppData/Local/Python/bin/python.exe" -m pip install pytest' } }

        stage('Test') { steps { bat '"C:/Users/user/AppData/Local/Python/bin/python.exe" -m pytest' } } 
    } 
}