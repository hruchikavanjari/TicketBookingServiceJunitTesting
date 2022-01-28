pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                bat 'mvn --version' 
            }
        }
        stage('--test--') {
            steps {
                bat "mvn test"
            }
        }
        stage('--package--') {
            steps {
                bat "mvn package"
            }
        }
    }
}

