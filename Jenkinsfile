pipeline {
    agent {
        label 'windows'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/karthick1409/jenkins-nodejs.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'npm test'
            }
        }

        stage('Build') {
            steps {
                echo 'Build complete (in this case, nothing to compile)'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage (could be Docker, SSH, etc.)'
            }
        }
    }
}
