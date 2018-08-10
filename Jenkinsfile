pipeline {
    agent { docker { image 'node:6.3' } }
    stages {
        stage('build') {
            echo "Docker Run ..."
            steps {
                    sh "docker-compose run nginx"
            }
        }
    }
}
