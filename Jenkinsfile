pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Demo Application'
        mvn  compile
      }
    }

    stage('Test') {
      steps {
        echo 'Test Demo Application'
        mvn  test
      }
    }

    stage('Deliver') {
      steps {
        echo 'Deliver  Demo Application'
        ./jenkins/scripts/deliver.sh
      }
    }

  }
}
