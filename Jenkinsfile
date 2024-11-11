pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello, World!'
                sh 'java -version'
            }
        }

        stage('Get directory details') {
            steps {
                sh 'pwd'
                sh 'ls -l'
            }
        }

        stage('Compile and Run Java') {
            steps {
                sh 'javac src/main/java/HelloWorld.java'
                sh 'ls'
                sh 'ls src/main/java'
                sh 'java src/main/java/HelloWorld'
            }
        }
    }
}
