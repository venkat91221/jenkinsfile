pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'update completed  successfully'
      }
    }
    stage('Shell') {
      steps {
        sh 'echo Hello World'
      }
    }
    stage('EMAIL') {
      steps {
        emailext(subject: 'Sample', body: 'Sample', to: 'root@localhost')
      }
    }
  }
}