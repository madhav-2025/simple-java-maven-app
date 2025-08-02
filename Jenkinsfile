pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/madhav-2025/simple-java-maven-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}

