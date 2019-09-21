
pipeline {
     agents any
     stages {
         stage ('Upload to AWS') {
             Steps {
                  withAWS(credentials: 'aws-static', region: 'us-west-2') {
                      s3Upload bucket: 'proj4', file: 'index.html'
                  }          
            }
        }
    }
}
