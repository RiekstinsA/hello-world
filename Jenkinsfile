pipeline {
    agent any
    parameters {
        string(name: 'NAME', defaultValue: 'WORLD', description: 'Person name')
    }
    stages {
        stage('Hello') {
            steps {
                echo "Hello ${params.NAME}"
            }
        }
        stage('Check node version') {
            steps {
                bat "node --version"
            }
        }
    }
}