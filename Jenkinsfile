pipeline {
    agent any

    stages {
        stage('Build') {
            
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