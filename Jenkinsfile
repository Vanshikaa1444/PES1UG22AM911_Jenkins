pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ main.cpp -o output'  // Compile C++ file
            }
        }
        stage('Test') {
            steps {
                sh './output'  // Run compiled output
            }
        }
        stage('Deploy') {
            steps {
                echo 'deploy'  // Simulating deployment step
            }
        }
    }
    post {
        failure {
            error 'Pipeline failed'  // Message when pipeline fails
        }
    }
}
