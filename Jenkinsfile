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
        sh './gradlew testDebugUnitTest'
      }
    }

    stage('Jacoco Code Coverage') {
      steps {
            sh 'chmod +x gradlew'
            sh './gradlew build -x test --no-daemon'
            sh './gradlew test jacocoTestReport --no-daemon'
        }
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
