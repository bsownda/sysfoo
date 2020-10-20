pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn compile'
      }
    }

    stage('Test') {
      steps {
        echo 'test maven app'
        sh 'mvn clean test'
      }
    }

    stage('Package') {
      steps {
        echo 'package maven app'
        sh 'mvn package -DskipTests'
        archiveArtifacts 'taget/*.war'
      }
    }

  }
  tools {
    maven 'Maven 3.6.3'
  }
}