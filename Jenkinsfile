pipeline{
    agent { dockerfile true }
    stages{
        stage('docker stage'){
            steps {
                sh 'echo FNAME=$FNAME'
            }
        }
    }
}