pipeline {
    agent any

    stages {
        stage('Build') {
            agent {
                docker {
                    image 'python:2-alpine'
                }
            }
            steps {
                sh 'ls'
                
                script {
                    def rootDir = pwd()
                    def example = load "${rootDir}@script/hello.Groovy "
                    example.hello()
                }
            }
        }
    }
}