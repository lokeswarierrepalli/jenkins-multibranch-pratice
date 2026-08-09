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
                echo 'GitHub Webhook Test'
            }
        }

        stage('Continous Deploy') {
            steps {
                echo 'Automatically deploying application...'
                echo 'Continous deployment successful'
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
