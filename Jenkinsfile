pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Vanshikaa1444/PES1UG22AM911_Jenkins.git'
            }
        }
        stage('Build') {
            steps {
                sh 'ls -l main'   // Debugging step to check if the file exists
                sh 'g++ main/hello.cpp -o main/output'  // Compile hello.cpp in the main folder
            }
        }
        stage('Test') {
            steps {
                sh './main/output'  // Run the compiled program
            }
        }
    }
}
