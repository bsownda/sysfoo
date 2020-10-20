pipeline{
  agent any

  tools{
    maven 'Maven 3.6.3'
  }

  stages{
      stage('Build'){
        steps{
            sh 'mvn compile'
        }
      } //Build stage
      stage('Test'){
        steps{
            sh 'mvn test'
        }
      } //test stage
      stage('Package'){
        steps{
            sh 'mvn package'
        }
    } //package stage
  } //stages
} //pipeline