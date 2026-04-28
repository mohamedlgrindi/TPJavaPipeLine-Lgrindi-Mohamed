pipeline {
    agent {
        docker {
            image 'maven:3.9.6-eclipse-temurin-17'
        }
    }

    stages {
        stage('Build Maven Project') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Run Java Program') {
            steps {
                sh 'mvn exec:java -Dexec.mainClass=Main'
            }
        }
    }
}