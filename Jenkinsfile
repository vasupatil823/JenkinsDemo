pipeline {
    agent any

    stages {
        stage('Build') {
                    steps {
                    withGradle {
                    sh '''
                                            ./gradlew clean build
                                            '''
                    }
                  }
                }
        stage('test') {
                            steps {
                            withGradle {
                            sh '''
                                                    ./gradlew test
                                                    '''
                            }
                          }
                        }
    }
}
