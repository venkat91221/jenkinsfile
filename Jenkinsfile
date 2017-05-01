pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'completed  successfully'
      }
    }
    stage('Shell') {
      steps {
        sh 'echo Hello Devops'
      }
    }
    stage('EMAIL') {
      steps {
        emailext(subject: 'Sample', body: 'Sample', to: 'root@localhost')
      }
    }
  }
}