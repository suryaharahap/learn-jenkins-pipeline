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
}