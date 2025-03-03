pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/sin14375/InClass3.git'
            }
        }

        stage('Build Java Project') {
            steps {
                sh 'javac src/main/java/com/sheridan/App.java'
            }
        }

        stage('Run Java Application') {
            steps {
                sh 'java -cp src com.sheridan.App'
            }
        }
    }
}
