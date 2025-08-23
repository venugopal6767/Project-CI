pipeline {
    agent any
    tools{
        maven 'maven3.9'
    }
    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/venugopal6767/Project-CI.git' 
            }
        }   
        stage('Maven compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('maven test') {
            steps {
                sh ' mvn test'
            }
        }
    }
}