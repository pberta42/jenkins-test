pipeline {
    agent any
    stages {
        stage('start') {
            steps {
                sh "pwd"
                sh "echo bruh"
                dir ('specs') {
                    git url: 'https://github.com/pberta42/jenkins-test2'
                }
                sh 'ls -la'
                load 'specs/Jenkinsfile'
            }
        }
    }
}
