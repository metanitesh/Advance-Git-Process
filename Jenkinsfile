pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "hello wolrd"'
        echo 'Start'
      }
    }

    stage('Lint') {
      steps {
        sh 'tidy -q -e *.html'
      }
    }

  }
}