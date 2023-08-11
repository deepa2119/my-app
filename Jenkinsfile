pipeline {
    agent any

    stages {
        stage('Clone and clean') {
            steps {
                sh "mvn clean -f my-app"
            }
        }
        stage('test') {
            steps {
                sh "mvn test -f my-app"
            }
        }
        stage('Package') {
            steps {
                sh "mvn package -f my-app"
            }
        }
    }
}
