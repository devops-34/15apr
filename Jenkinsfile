pipeline {
    agent any
    stages {
        stage('---clean---') {
            steps {
                sh " sudo yum install update"
                sh "sudo yum install maven -y"
                sh "sudo systemctl enable maven" 
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
