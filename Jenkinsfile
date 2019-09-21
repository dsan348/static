
pipeline {
     agent any
     stages {
         stage ('Upload to AWS') {
             steps {
                  withAWS(credentials: 'aws-static', region: 'us-west-2') {
                      s3Upload bucket: 'proj4', file: 'index.html'
                  }          
            }
        }
    }
}
