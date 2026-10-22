pipeline {
    agent any
    tools{
        jdk 'jdk-17'
        maven 'maven-3.10'
    }
 
    stages {
        stage('Git checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Bhupeshh2906/Boardgame.git'
            }
        }
        stage('code compilation using maven') {
            steps {
                sh 'mvn compile'
            }
        }
         stage('code run test cases using maven') {
            steps {
                sh 'mvn test'
            }
        }
         stage('code build using maven') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
