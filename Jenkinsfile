pipeline {
    agent any

    tools {
        maven 'Maven 3.9.4'  // ✅ match exactly with Jenkins Maven name
        jdk 'JDK22'          // ✅ also make sure 'JDK22' exists under Global Tool Config
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
