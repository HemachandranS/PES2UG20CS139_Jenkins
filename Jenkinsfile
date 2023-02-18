pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS181-1 working.cpp'
                echo 'BuildiNG successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS181-1'
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
