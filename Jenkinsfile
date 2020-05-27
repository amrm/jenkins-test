pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'this build number $BUILD_NUMBER with demo $Demo'
        sh 'echo "this build number $BUILD_NUMBER with demo $Demo"'
      }
    }

  }
  environment {
    Demo = '1'
  }
}