pipeline {
  agent any
  options {
    timestamps()
    skipStagesAfterUnstable()
  }
  stages {
    stage('Build') {
      steps {
        echo "This is an example of skipStagesAfterUnstable"
        script {
          currentBuild.result = 'UNSTABLE'
        }
      }
    }
    stage('Test') {
      steps {
        echo "Hello world from Testing phase"
      }
    }
    stage('Deploy') {
      steps {
        echo "Hello world from Testing phase"
      }
    }
  }
  
