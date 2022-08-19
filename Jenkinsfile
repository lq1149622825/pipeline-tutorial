pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building spring boot'
                sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
        stage('sonar') {
             steps {
                echo 'Deploying....'
             }
        }
    }
}
