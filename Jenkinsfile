pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh " yum install update -y"
            }
        }
        stage('--test--') {
            steps {
                sh "mvn test"
            }
        }
        stage('--package--') {
            steps {
                sh "mvn package"
            }
        }
    }
}
