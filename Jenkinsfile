pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '# build'
      }
    }
    stage('Result') {
      parallel {
        stage('Result') {
          steps {
            echo 'result'
          }
        }
        stage('Result1') {
          steps {
            echo 'result2'
          }
        }
      }
    }
    stage('test') {
      steps {
        echo 'message'
        echo 'aaaa'
      }
    }
    stage('result') {
      steps {
        sh 'echo "last" result'
      }
    }
  }
}