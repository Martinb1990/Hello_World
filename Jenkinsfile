pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                echo 'Hello world!'
            }
        }
        stage('Test') {
            steps {
                bat 'make check || true'
                junit '**/target/*.xml'
            }
        }
    }
}
