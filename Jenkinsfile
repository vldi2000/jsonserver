pipeline {
  agent none
  stages {
    stage('run') {
      steps {
        sh 'pytest my_basic_test.py --headless'
      }
    }

  }
}