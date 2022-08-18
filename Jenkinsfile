pipeline {
    agent any
    stages {
        stage ('packaging the application') {
            steps {
                echo 'packaging'
            }
        }
        stage ('sonarqube analysis') {
            when {
                branch "dev"
            }
            steps {
                echo 'skipping'
            }
        }
    }
}
