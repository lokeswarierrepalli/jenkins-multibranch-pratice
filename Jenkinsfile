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
       stage('Docker Deployment') {
    steps {
        sh 'docker build -t jenkins-demo:latest .'
        sh 'docker rm -f jenkins-demo || true'
        sh 'docker run -d --name jenkins-demo -p 8080:80 jenkins-demo:latest'
        echo 'Docker deployment completed successfully'
    
            }
        }
    }

    post {
        success {
            echo 'Multibranch Pipeline completed successfully'
        }
    }
}
