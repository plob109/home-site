pipeline {
    agent any
    tools{
        nodejs '18.9.1 Installed'
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                //sh 'npm run build'
                sh 'npm --version'
                sh 'npm run docker:build'
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
                sh 'npm run docker:run'
            }
        }
    }
}
