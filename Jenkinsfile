pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                bat 'g++ -o hello_exec.exe main\\hello.cpp'
            }
        }
        stage('Test') {
            steps {
                bat '.\\hello_exec.exe'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment Stage (Placeholder)'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
