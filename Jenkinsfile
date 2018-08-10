pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                script{
                    docker.image('node:6.3').inside{ 
                        sh 'pwd'
                        sh 'ls'
                    }
                }
            }
        }
    }
}
