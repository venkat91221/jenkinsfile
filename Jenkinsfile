pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        parallel(
          "Stage1": {
            echo 'Heloo World'
            
          },
          "": {
            echo 'Hello Step22'
            
          }
        )
      }
    }
    stage('Stage2') {
      steps {
        sleep 5
      }
    }
    stage('EMAIL') {
      steps {
        emailext(subject: 'Sample', body: 'Sample', to: 'root@localhost')
      }
    }
  }
}