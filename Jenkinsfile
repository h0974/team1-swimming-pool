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
                SONAR_TOKEN = credentials('sonarqube-token')
            }
            steps {
                sh '''./gradlew sonarqube \
                    -Dsonar.projectKey=user46-swimming-pool \
                    -Dsonar.host.url=http://140.134.26.54:10990 \
                    -Dsonar.login=df233984af96a39849aa4efcda6b749e78afbd88
                '''
            }
        }
    }
    
}