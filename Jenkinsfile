pipeline {
    agent any

    stages {
        stage('SCM Checkout') {
            steps {
                echo 'Checking out Jenkinsfile from GitHub'
            }
        }

        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/madhav-2025/simple-java-maven-app.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project using Maven'
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}

