pipeline {
    agent { label 'windows' } // 👈 Change to match your Windows node label

    stages {
        stage('Preparation') {
            steps {
                echo '✅ Running on Windows Agent'
                bat 'ver'            // Print Windows version
                bat 'where node'     // Verify Node.js is installed
                bat 'where npm'      // Verify npm is installed
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests') {
            steps {
                bat 'npm test'
            }
        }

        stage('Done') {
            steps {
                echo '✅ Build finished on Windows node.'
            }
        }
    }
}
