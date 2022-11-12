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
        }             
        stage('Testing maven') {
            steps {
                sh """mvn -version"""
        }
    }
      stage('MVN CLEAN') {
            steps {
                sh 'mvn clean'
        }
    }
         stage('MVN COMPILE') {
            steps {
                sh 'mvn compile'
        }
    }
             stage('MVN SONARQUBE') {
            steps {
                sh 'mvn sonar:sonar -Dsonar.login=admin -Dsonar.password=sonar -DskipTests'
        }
    }
}
}
