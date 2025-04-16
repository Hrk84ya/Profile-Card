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
                sh 'npm install -g htmlhint || true'
                sh 'htmlhint index.html || true'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                sh 'mkdir -p $HOME/html-deploy/myproject'
                sh 'cp -r * $HOME/html-deploy/myproject/'
            }
        }
    }
}