pipeline{
    agent {
        docker { image 'node:14-alpine' }
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