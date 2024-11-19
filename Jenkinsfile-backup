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
                                   test -f build/libs/demo-0.0.1-SNAPSHOT.jar
                                                    '''
                          }
                        }
    }
}
