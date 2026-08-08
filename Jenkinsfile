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
                echo 'poll SCM Test 2'
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
