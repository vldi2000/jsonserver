pipeline {
  agent {
    docker {
      image 'seleniumbase'
    }

  }
  stages {
    stage('run') {
      steps {
        sh '''docker run seleniumbase ./run_docker_test_in_chrome.sh
'''
      }
    }

  }
}