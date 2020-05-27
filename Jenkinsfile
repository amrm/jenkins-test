pipeline {
  agent any
  stages {
    stage('hello') {
      steps {
        echo 'Hello World'
        sh 'echo "this build number $BUILD_NUMBER with demo $Demo"'
      }
    }

     stage('clean') {
          steps {
            sh ' echo "clean ..." '

          }
        }

         stage('install') {
                  steps {
                    sh ' echo "install ..." '
                  }
                }

                 stage('Build') {
                                  steps {
                                    sh ' echo "Build ..." '
                                  }
                                }
}
  environment {
    Demo = '2'
  }
}
