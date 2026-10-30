
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Flyway Validate') {
            steps {
                bat 'flyway validate'
            }
        }

        stage('Flyway Migrate') {
            steps {
                bat 'flyway migrate'
            }
        }
    }
}
