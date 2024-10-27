pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Building Demo Application'
        sh 'mvn clean compile'
      }
    }

    stage('Test') {
      steps {
        echo 'Testing Demo Application'
        sh 'mvn test'
      }
    }

    stage('Deliver') {
      steps {
        echo 'Delivering Demo Application'
        sh './jenkins/scripts/deliver.sh'
      }
    }
  }
}
