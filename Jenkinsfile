pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'gradle clean build'
      }
    }
    stage('Test') {
      steps {
        bat 'gradle test'
      }
    }
    stage('SonarQube') {
      steps {
        bat 'gradle sonarqube'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy the Project'
      }
    }
    stage('Release') {
      steps {
        echo 'Project was successfully Released'
      }
    }
  }
}