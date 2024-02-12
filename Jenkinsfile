pipeline {
    agent any
    stages {
        stage('Prebuild Stage') {
            echo "Pre-Build Stage"
            steps {
                script {
                    load 'vars/buildPipeline.groovy'
                }
            }
        }
    }
}