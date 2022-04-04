pipeline {
    agent any

    tools {
            maven 'Maven 3.6.2'
        }

    stages {
        stage('Pull') {
            steps {
                git 'https://github.com/asrwy/jenkins-demo.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Push') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
