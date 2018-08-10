pipeline {
    agent { docker { 
                image 'node:6.3' 
                args '-v  /var/jenkins_home/workspace/learn:/usr/src/app -w /usr/src/app'
                reuseNode true
            } 
     }
    stages {
        stage('build') {
            steps {
                sh 'npm --version'
                sh 'ls /usr/src/app'
                sh 'docker run --rm -v /usr/src/app:/aa busybox ls /aa' 
            }
        }
    }
}
