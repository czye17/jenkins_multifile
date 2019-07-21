pipeline {
    agent any

    stages {
        stage('Build') {

            steps {
                sh 'ls'

                script {
                    def example = load "hello.Groovy"
                    example.hello()
                }
            }
        }
    }
}