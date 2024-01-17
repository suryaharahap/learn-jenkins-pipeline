pipeline {
  agent {
    node {
      label "linux && java21"
    }
  }
  stages {
    stage('hello') {
      steps {
        echo 'hello jenkins pipeline in the world.'
      }
    }
  }

  post {
    always {
      echo 'I will always say hello again!'
    }
    success {
      echo 'Yay, success'
    }
    failure {
      echo 'Oh no, failure'
    }
    cleanup {
      echo "Don't care success or error"
    }
  }
}