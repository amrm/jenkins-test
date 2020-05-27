pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'this build number $BUILD_NUMBER with demo $Demo'
        sh 'echo "this build number $BUILD_NUMBER with demo $Demo"'
      }
    },

      stage('step2') {
          withMaven(maven: 'mvn') {
             sh "mvn clean package"
          }
        }

  }
  environment {
    Demo = '2'
  }
}
