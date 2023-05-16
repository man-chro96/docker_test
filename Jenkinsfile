pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                // Checkout source code from Git repository
                git 'https://github.com/dimosko/jenkins-hello-world.git'
                
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