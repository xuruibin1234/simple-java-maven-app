pipeline {
    agent {
        docker {
            image 'maven:3.8.1-jdk-8-alpine'
            args '-v F:\\apache-maven-3.9.9\\repository:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -B -DskipTests clean package'
            }
        }
    }
}