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

        stage('Rolling Deployment') {
    steps {
        echo 'Deploying to server 1...'
        echo 'Server 1 deployment successful'

        echo 'Deploying to server 2...'
        echo 'Server 2 deployment successful'

        echo 'Deploying to server 3...'
        echo 'Server 3 deployment successful'

        echo 'Rolling deployment completed successfully'
    
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
