pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Compiling project'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests'
            }
        }

    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
