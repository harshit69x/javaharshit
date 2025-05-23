pipeline {
    agent any

    tools {
        maven 'Maven 3.9.6' // or whatever version name you configured in Jenkins
        jdk 'JDK22'         // match the JDK name from Global Tool Config
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/harshit69x/javaharshit.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
