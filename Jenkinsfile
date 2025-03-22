pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o pes1ug23cs833 main/hell.cpp'
                echo 'Build stage completed successfully'
            }
        }
        
        stage('Test') {
            steps {
                sh './pes1ug23cs833'
                echo 'Test stage completed successfully'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deployment stage completed successfully'
                echo 'Deployed the application'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
        success {
            echo 'Pipeline executed successfully'
        }
    }
}V
