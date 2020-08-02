pipeline{
    agent any
    stages{
        stage('build'){
            steps{
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
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