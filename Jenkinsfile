pipeline {
  agent any
  stages {
    stage('version check') {
      steps {
        sh '''mvn --version
java --version'''
      }
    }

    stage('UT') {
      steps {
        sh 'mvn test'
      }
    }

    stage('build') {
      steps {
        sh 'mvn package'
      }
    }

  }
}