pipeline {
    agent { label 'windows' } // 👈 Replace with your actual Windows agent label

    stages {
        stage('Say Hello') {
            steps {
                echo 'Starting Hello World Pipeline on Windows Node...'
                bat 'echo Hello, World!'
            }
        }
    }
}
