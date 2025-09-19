pipeline {
    agent {
        label 'windows'
    }

    tools {
        nodejs 'NodeJS_18' // Adjust to match your Jenkins NodeJS tool name
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-username/simple-node-app.git'
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
