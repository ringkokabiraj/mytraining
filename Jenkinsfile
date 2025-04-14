pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ringkokabiraj/mytraining.git'
            }
        }

        stage('Read hello.txt') {
            steps {
                script {
                    def content = readFile('hello.txt')
                    echo "Content of hello.txt:\n${content}"
                }
            }
        }
    }
}