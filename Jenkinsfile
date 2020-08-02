pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo "build stage"
                sh 'make'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
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