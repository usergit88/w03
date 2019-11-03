
pipeline {
    agent {
        dockerfile {
            filename 'Dockerfile.jenkinsAgent'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    

pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
