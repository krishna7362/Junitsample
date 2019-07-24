pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/balajireddy8898/Junitsample.git', branch: 'master')
      }
    }
    stage('compile') {
      steps {
        bat 'mvn compile'
      }
    }
    stage('JunitTest') {
      steps {
        bat 'mvn test'
      }
    }
    stage('Build') {
      steps {
        bat 'mvn clean install'
        bat 'mvn clean install'
      }
    }
  }
}