pipeline {
  agent any
  stages {
    stage('Build') {
      steps{
        sh """
           gradle clean assembleDebug
           """
      }
    }

    stage('Unit Test') {
      steps {
        echo "Unit Test Dummy"
      }
    }

    stage('Jacoco Code Coverage') {
      steps {
        echo "Jacoco Code Coverage Dummy"
      }
    }

    stage('Lint Checks') {
      steps {
        echo "Lint Checks Dummy"
      }
    }

    stage('Code Quality') {
      steps {
        echo "Lint Checks Dummy"
      }
    }

    stage('UI test Android') {
      steps {
        echo "UI test Android Dummy"
      }
    }
  }
  post {
    always {
      echo 'Cleaning workspace...'
    }
  }
}
