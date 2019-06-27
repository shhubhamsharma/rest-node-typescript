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
                bat 'npm run build'
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
    post {
        always {
            archiveArtifacts artifacts: 'dist/*.js', fingerprint: true
        }
    }
}