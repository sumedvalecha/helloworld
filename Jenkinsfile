pipeline {
    agent {
        docker {
            image 'python:3.11'
        }
    }
    stages {
        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Run Script') {
            steps {
                sh 'python main.py'
            }
        }
    }
}
