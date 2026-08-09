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
       stage('Canary Deployment') {
    steps {
        echo 'Deploying new version to 10% of users...'
        echo 'Monitoring canary deployment...'
        echo 'Canary is healthy'

        input message: 'Approve rollout to 100% of users?', ok: 'Rollout'

        echo 'Rolling out new version to 100% of users...'
        echo 'Canary deployment completed successfully'
        
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
