pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Cloning source code...'
                checkout scm
            }
        }

        stage('Lint HTML') {
            steps {
                echo 'Validating HTML...'
                // Optional: Install and run htmlhint or any linter
                sh 'npm install -g htmlhint || true'
                sh 'htmlhint index.html || true'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Example: Copy to a directory or use scp/ftp/deploy tool
                sh 'mkdir -p /var/www/html/myproject'
                sh 'cp -r * /var/www/html/myproject/'
            }
        }
    }
}