pipeline {
    agent any
    stages {
        stage('Clean') {
            steps {
                script{
                    sh "./mvnw clean"
                }
            }
        }

        stage('Compile') {
            steps {
                script{
                    sh "./mvnw compile"
                }
            }
        }

        stage('Test') {
            steps {
                script{
                    sh "./mvnw test"
                }
            }
        }
    }
}
