pipeline {
    agent any

    stages {
        stage('Checkout Git') {
            steps {
                echo 'Hello World'
            }
        }
        
        stage('Hello') {
            steps {
                echo 'pulling...';
              git branch: 'master',
                url:'https://github.com/ChaimaBenAbdelaziz/IOC.git';
            
        }
             
        stage('Testing maven') {
            steps {
                sh """mvn -version"""
          
        }
    }
}

