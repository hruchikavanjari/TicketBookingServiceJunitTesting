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
               git pull origin master
            }
        }
        stage('--package--') {
            steps {
                yarn build
            }
        }
    }
}

