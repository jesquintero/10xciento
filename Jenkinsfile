pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                mvn wrapper:wrappe
                sh  "chmod +x mvnw"
                sh "mvnw clean"
            }
        }

        stage('Compile') {
            steps {
                mvn wrapper:wrappe
                sh  "chmod +x mvnw"
                sh "mvnw compile"
            }
        }

        stage('Test') {
            steps {
                mvn wrapper:wrappe
                sh  "chmod +x mvnw"
                sh "mvnw test"
            }
        }
    }
}
