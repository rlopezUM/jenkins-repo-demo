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
                sh 'ls'
                sh 'ls src/main/java'
                dir('src/main/java') {
                    sh 'javac HelloWorld.java'
                    sh 'java HelloWorld'
                }
            }
        }
    }
}
