pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Test successful'
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
