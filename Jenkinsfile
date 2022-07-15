pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('') {
      steps {
        sh 'ls'
        sleep 2
        sh 'echo "world"'
        retry(count: 3) {
          echo 'kmkmk'
        }

        sh 'kkkk'
      }
    }

  }
}