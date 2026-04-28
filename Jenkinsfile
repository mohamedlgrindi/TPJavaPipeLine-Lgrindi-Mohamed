pipeline {
    agent any

    stages {

        stage('Verify Maven') {
            steps {
                sh 'mvn -version'
            }
        }

        stage('Build Maven Project') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run Java Program') {
            steps {
                sh 'java -cp target/classes Main'
            }
        }
    }
}