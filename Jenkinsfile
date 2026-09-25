pipeline {

    agent any

    stages {

        stage('Tests JUnit') {

            steps {

                sh './mvnw test'
            }

            post {

                always {

                    junit 'target/surefire-reports/*.xml'
                }
            }
        }
    }
}