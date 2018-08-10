pipeline {
    agent node
    stages {
        stage('build') {
            steps {
                    sh "docker run --rm -v '${env.WORKSPACE}':'/project':ro  busybox ls /project"
                    sh "docker-compose run nginx"
            }
        }
    }
}
