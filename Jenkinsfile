pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Mary'
  }
}