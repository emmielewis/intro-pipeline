library 'SharedLibs'
pipeline {
  agent any
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${params.Name}!"
      }
    }
    stage('Shared Lib') {
         steps {
             helloWorld("Jenkins")
         }
      }
  }
  environment {
MY_NAME = 'Mary'
}

  post {
    aborted {
      echo 'Why did you not push my button?'
    }
  }
}
