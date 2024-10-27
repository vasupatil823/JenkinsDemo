pipeline {
    agent any

    stages {
        stage('Build') {
                    steps {
                        // Use Gradle wrapper or Gradle directly
                        sh './gradlew clean build' // If using Gradle wrapper
                        // Or alternatively, without wrapper:
                        // sh 'gradle clean build'
                    }
                }
    }
}
