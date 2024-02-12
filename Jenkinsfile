pipeline {
    agent any
    stages {
        stage('Build & deploy') {
            steps {
                script {
                    load 'vars/buildPipeline.groovy'
                }
            }
        }
    }
}