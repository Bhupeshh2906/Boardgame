pipeline {
    agent any
    tools{
        jdk 'jdk-17'
        maven 'maven-3.10'
    }
    stages {
      stage('compile') {
              steps {
                  sh 'mvn compile'
              }
          }
      stage('test') {
              steps {
                  sh 'mvn test'
              }
          }
      stage('build') {
              steps {
                  sh 'mvn package'
              }
          }
      }
  }
