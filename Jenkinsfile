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
        sh 'sh \'tidy -q -e *.html\''
      }
    }

  }
}