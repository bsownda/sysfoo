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
            echo 'test maven app'
            sh 'mvn clean test'
        }
      } //test stage
      stage('Package'){
        steps{
            echo 'package maven app'
            sh 'mvn package -DskipTests'
        }
    } //package stage
  } //stages
} //pipeline