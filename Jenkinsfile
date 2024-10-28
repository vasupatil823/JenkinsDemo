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
        stage('Test') {
                            steps {
                            sh '''
                                   echo "Test stages"
                                                    '''
                          }
                        }
    }
}
