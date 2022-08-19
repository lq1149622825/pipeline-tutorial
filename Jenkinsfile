pipeline {
    agent any

      environment {
        SONAR_TOKEN = credentials('sonar-token')
      }

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
                  -Dsonar.host.url=http://192.168.3.8:9000 \
                  -Dsonar.login=$SONAR_TOKEN
                  '''
             }
        }
    }
}
