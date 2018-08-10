pipeline {
    agent { docker { 
                image 'node:6.3' 
                args '-v ${PWD}:/usr/src/app -w /usr/src/app'
                reuseNode true
            } 
     }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
                sh 'ls /usr/src/app'
                sh 'docker images'
                sh 'pwd'
                sh 'docker run --rm -v /:/aa busybox ls /aa' 
            }
        }
    }
}
