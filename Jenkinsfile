pipeline {
  agent any
  stages {
    stage('1') {
      steps {
        sh 'echo "hello"'
      }
    }

    stage('error') {
      steps {
        sh 'ls'
        sleep 2
        sh 'echo "world"'
        retry(count: 3) {
          echo 'kmkmk'
        }

        input(message: '123', id: 'id', ok: 'ok', submitter: 'Submitter', submitterParameter: 'SubmitterParameter')
        sh 'echo "123"'
      }
    }

  }
}