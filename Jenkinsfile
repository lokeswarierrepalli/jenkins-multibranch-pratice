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

        stage('Continuous Delivery') {
    steps {
        echo 'Build and tests completed'
        input message: 'Approve release to production?', ok: 'Release'
        echo 'Release ready for production'
    
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
