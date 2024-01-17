pipeline {
  agent {
    node {
      label "linux && java21"
    }
  }
  stages {
    stage('Build') {
      steps {
        echo 'hello build'
      }
    }

    stage('Test') {
      steps {
        echo 'hello test'
        sh('error')
      }
    }

    stage('Deploy') {
      steps {
        echo 'hello deploy'
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