pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Checkout source code from Git repository
                git 'https://github.com/man-chro96/docker_test.git'
                
                // Build step using GCC
                sh 'gcc -o hello hello.c'
            }
        }

        stage('Execute') {
            steps {
                // Execute the compiled program
                sh './hello'
            }
        }
    }
}