pipeline {
  agent any
  stages {
    stage('Build') {
      steps{
        sh './gradlew clean assembleDebug'
      }
    }

    stage('Unit Test') {
      steps {
        sh './gradlew app:testDummyDebugUnitTest'
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
