pipeline{
    agent {
        docker { image: 'nginx:latest' }
    }
    stages{
        stage('build'){
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