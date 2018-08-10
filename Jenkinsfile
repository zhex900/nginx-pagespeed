pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                    sh "ls"
                    sh "docker run --rm -v '${env.WORKSPACE}':'/project'  busybox cat /project/Dockerfile"
                    sh "docker-compose run nginx"
            }
        }
    }
}
