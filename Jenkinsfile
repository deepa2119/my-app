pipeline {
    agent any

    stages {
        stage('Clone and clean') {
            steps {
                sh "rm -rf my-app"
                sh "git clone https://github.com/deepa2119/my-app.git"
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
