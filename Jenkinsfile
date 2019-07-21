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
                script {
                    def example = load "${rootDir}@script/hello.Groovy "
                    example.hello()
                }
            }
        }
    }
}