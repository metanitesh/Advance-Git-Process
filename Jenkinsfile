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
    
    stage('Upload to AWS') {
        steps {
          
            s3Upload(pathStyleAccessEnabled:true, payloadSigningEnabled: true, file:'index.html', bucket:'jenkins-s3-nitesh')
         
     }

  }
}
