pipeline {
    agent any

    tools {
        maven 'Maven-3'  // Must match the name you gave in Step 1
        // jdk 'JDK-17'  // Uncomment and add if you configured a JDK tool as well
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