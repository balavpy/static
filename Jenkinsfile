pipeline {
    agent any

    stages {
            stage ('lint html') {
                steps {
                    sh 'tidy -q -e *.html'
                }
            }
           stage('Upload to AWS') {
                 steps {
                    withAWS(region:'us-east-1',credentials:'aws-static') {
                    s3Upload(file:'index.html', bucket:'balavpyudacity')
                    echo 'File successfully uploaded into S3'
                 }

            }
        }
    }
}
