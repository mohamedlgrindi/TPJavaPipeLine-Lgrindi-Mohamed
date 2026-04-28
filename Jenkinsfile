pipeline {
    agent any
    
    tools {
        maven 'Maven-3'
        jdk 'JDK-17'
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