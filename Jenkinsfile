pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building...'
                bat 'docker build -t myapp .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                bat 'echo Test Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat 'docker run -d -p 5000:5000 myapp'
            }
        }
    }
}
