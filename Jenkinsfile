pipeline {
  agent any
  stages {
    stage('hoge') {
      steps {
        sh 'echo "hoge"'
      }
    }
    stage('huga') {
      steps {
        sh 'echo "huga"'
      }
    }
    stage('fail test') {
      steps {
        sh 'hogehoge'
      }
    }
    stage('echo hostname') {
      steps {
        sh 'hostname'
      }
    }
  }
  post {
    always {
      sh 'echo "DONE"'
    }
  }
}
