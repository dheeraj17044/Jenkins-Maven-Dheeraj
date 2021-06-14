pipeline {
    agent any
    tools {
        jdk 'JDK11'
    }
    stages {
        stage('build') {
            steps {
                echo 'Started Build'
                bat 'mvn --version'
                bat 'mvn clean compile'
                echo 'Compiled Build Succesfully'
                bat 'mvn test'
                echo 'Finished Build Testing Succesfully'
                bat 'mvn package'
                echo 'Finished Build Succesfully'
            }
        }
    }
}