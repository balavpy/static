pipeline{
    agent {
        docker { image 'alpine:latest' }
    }
    stages{
        stage('dockerbuild'){
            steps{
                sh 'node --version'
            }
        }
        stage('test'){
            steps{
                echo "test stage"
            }
        }
        stage('deploy'){
            steps{
                echo "deploy stage"
            }
        }
    }
}