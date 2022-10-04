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
