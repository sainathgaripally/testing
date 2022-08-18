pipeline {
    agent any
    environment {
        PATH= "$PATH:/usr/share/maven"
    }
    stages {
        stage ('packaging the application') {
            steps {
                sh 'mvn clean package'
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
