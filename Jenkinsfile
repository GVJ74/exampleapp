pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'npm i'
            }
        }
        stage('Deploy') {
            steps {
                parallel {
                    a: {bat 'npm run build'}
                    b: {bat 'npx json-server path/to/file --port 8000'}
                }
            }
        }
    }
}
