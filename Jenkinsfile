pipeline {
    agent any
    
    stages {
        stage('run-test') {
            steps {
               ...(略)…
                )
            }
        }

        stage('sonarqube-analysis') {
            environment {
                SONAR_TOKEN = credentials('{sonarqube-token}')
            }
            steps {
                sh '''./gradlew sonarqube \
                    -Dsonar.projectKey={user46-swimming-pool
master} \
                    -Dsonar.host.url=http://140.134.26.54:10990 \
                    -Dsonar.login=$SONAR_TOKEN
                '''
            }
        }
    }
}
