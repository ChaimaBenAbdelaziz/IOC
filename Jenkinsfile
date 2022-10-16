pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
          stages {
        stage('Hello') {
            steps {
                echo 'pulling...';
              git branch: 'master',
                url:'https://github.com/ChaimaBenAbdelaziz/IOC.git';
            }
        }
                stages {
        stage('Testing maven') {
            steps {
                sh """mvn -version"""
            }
        }
    }
}

