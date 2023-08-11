pipeline {
    agent any

    stages {
        stage('Clone and clean') {
            steps {
                sh "mvn clean"
            }
        }
        stage('test') {
            steps {
                sh "mvn test"
            }
        }
        stage('Package') {
            steps {
                sh "mvn package"
            }
        }
    }
}
