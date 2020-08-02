pipeline{
    agent {
        docker { image 'nginx:latest' }
    }
    stages{
        stage('dockerbuild'){
            steps{
                sh 'uname -a'
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