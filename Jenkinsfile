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
                bat 'mvn exec:java -Dexec.mainClass=Main'
            }
        }
    }
}