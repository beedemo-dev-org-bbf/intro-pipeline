pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PWS}"
      }
    }
  }
  environment {
    MY_NAME = 'Bibiana'
    TEST_USER = credentials('test-user')
  }
}