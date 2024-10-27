pipeline {
    agent any
    stages {
        stage('Build') {
        agent {
                        docker {
                            image 'openjdk:17-oracle'
                        }
                    }
                    steps {
                        sh '''
                        ls -la
                        java --version
                        gradle clean build
                        ls -la
                        '''
                    }
                }
    }
}
