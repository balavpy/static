pipeline {
    agent any

    stages {
        stage('Upload to AWS') {
            withAWS(region:'us-east-1',credentials:'aws-static') {
               s3Upload(file:'index.html', bucket:'balavpyudacity', path:'path/to/target/index.html')
            }
            steps {
                echo 'File successfully uploaded into S3
            }
        }
    }
}
