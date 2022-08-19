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
                sh '''
                   ./gradlew sonarqube \
                  -Dsonar.projectKey=pipeline \
                  -Dsonar.host.url=http://0.0.0.0:9000 \
                  -Dsonar.login=jenkins
                  '''
             }
        }
    }
}
