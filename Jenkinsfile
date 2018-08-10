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
                sh 'ls'
                sh 'docker run --rm -v $(pwd):/aa busybox ls /aa' 
            }
        }
    }
}
