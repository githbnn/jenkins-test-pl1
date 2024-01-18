pipeline {
    agent { docker { image 'node:20.11.0-alpine3.19' } }
    stages {
        stage('Initialize'){
        steps {
                def dockerHome = tool 'myDocker'
                env.PATH = "${dockerHome}/bin:${env.PATH}"
                }        
        }
        stage('build') {
        steps {
                sh 'node --version'
            }
        }
    }
}
