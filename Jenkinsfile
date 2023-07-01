pipeline {
  agent any
  stages {
    stage('run') {
      steps {
        sh 'pytest my_basic_test.py --headless'
      }
    }

  }
}