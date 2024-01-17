pipeline {
  agent {
    node {
      label "linux && java21"
    }
  }
  stages {
    stage('Build') {
      steps {
        echo 'hello build one'
        sleep(10)
        echo 'hello build two'
        echo 'hello build three'
      }
    }

    stage('Test') {
      steps {
        echo 'hello test one'
        sleep(10)
        echo 'hello test two'
        echo 'hello test three'
      }
    }

    stage('Deploy') {
      steps {
        echo 'hello deploy one'
        sleep(10)
        echo 'hello deploy two'
        echo 'hello deploy three'
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