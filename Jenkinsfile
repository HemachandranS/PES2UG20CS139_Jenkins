pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh ' -o PES2UG20CS139-1 working.cpp'
                echo 'BuildiNG successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS139-1'
                echo 'Testing successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying successful'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
