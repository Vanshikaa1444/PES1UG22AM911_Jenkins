pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Vanshikaa1444/PES1UG22AM911_Jenkins.git'
            }
        }
        stage('Build') {
            steps {
                sh 'g++ main/hello.cpp -o main/output'
            }
        }
        stage('Test') {
            steps {
                sh './main/output'
            }
        }
    }
}
