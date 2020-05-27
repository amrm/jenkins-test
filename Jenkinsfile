pipeline {
  agent any
  tools {
          maven 'Maven 3.3.9'
          jdk 'jdk8'
      }
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
            sh ' mvn clean '
          }
        }

         stage('install') {
                  steps {
                    sh ' echo "install ..." '
                    sh ' mvn install '
                  }
                }

                 stage('Build') {
                                  steps {
                                    sh ' echo "Build ..." '
                                    sh ' mvn build '
                                  }
                                }
}
  environment {
    Demo = '2'
  }
}
