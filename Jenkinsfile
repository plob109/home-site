pipeline {
    agent any
    tools{
        nodejs '18.9.1 Installed'
    }
    stages {
        stage('requirement install') {
            steps {
                sh 'npm install -g gatsby-cli'
            }
        }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'pwd'
                sh 'gatsby --version'
                sh 'gatsby build'
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
