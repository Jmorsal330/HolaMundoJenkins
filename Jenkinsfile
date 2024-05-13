pipeline {
    agent any
    tools {
        maven "Maven 3.6.3"
        jdk "JDK11"
    }
    stages {
        stage('env') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('build') {
            steps {
                sh 'mvn clean install -B --no-transfer-progress'
            }
        }
    }
}