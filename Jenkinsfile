pipeline {
    agent any

    stages {
        stage('Build Maven Project') {
            steps {
                bat 'mvn clean package'
            }
        }

        stage('Run Java Program') {
            steps {
                bat 'java -cp target\\classes Main'
            }
        }
    }
}