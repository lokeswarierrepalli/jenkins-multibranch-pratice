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

        stage('Blue-Green Deployment') {
    steps {
        echo 'Blue environment: current production'
        echo 'Green environment: deploying new version'
        echo 'Testing Green environment...'
        echo 'Green environment is healthy'
        input message: 'Switch traffic from Blue to Green?', ok: 'Switch'
        echo 'Traffic switched from Blue to Green'
        echo 'Blue-Green deployment successful'
    
    
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
