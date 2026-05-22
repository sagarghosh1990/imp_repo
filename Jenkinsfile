pipeline {
    agent any

    environment {
        PYTHON = 'C:\\Users\\MONY SAGAR GHOSH\\AppData\\Roaming\\Microsoft\\Windows\\Start Menu\\Programs\\Python 3.14'
    }
    stages {
        stage("checkout code") {
            steps {
                checkout scm
            }
            
        }
        stage('show python version') {
            steps {
                bat "\"${env.PYTHON}\" --version"
            }
        }
        stage('run extract_data.py') {
            steps {
                bat "\"${env.PYTHON}\" extract_data.py"
            }
        }
    }
}