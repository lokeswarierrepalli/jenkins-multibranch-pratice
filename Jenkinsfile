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

        stage('Manual Deploy') {
            steps {
                input message: 'Deploy to production?', ok: 'Deploy'
                echo 'Manual deployment successful'
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
