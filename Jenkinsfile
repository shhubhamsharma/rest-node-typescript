pipeline {
    agent any

    stages {
                stage('PreBuild') {
            steps {
                echo 'Installing Dependencies..'
                bat 'npm i'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                bat 'npm run prod'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}