pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                dir('integrationwithjenkins') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('integrationwithjenkins') {
                    sh 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('integrationwithjenkins') {
                    sh 'mvn package'
                }
            }
        }
    }
}