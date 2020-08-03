pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v vol:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B'
            }
        }
    }
}