pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'pip install flask'
            }
        }
        stage('Deploy') {
            steps {
                sh 'python3 app.py'
            }
        }
    }
}