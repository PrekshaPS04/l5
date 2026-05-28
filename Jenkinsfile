pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch : 'main',url : 'https://github.com/PrekshaPS04/l5.git'
            }
        }
        stage('Install') {
            steps {
                bat 'npm install'
            }
        }
        stage('run app') {
            steps {
                bat 'npm app.js'
            }
        }
        stage('run test') {
            steps {
                bat 'npm test.js'
            }
        }
    }
}