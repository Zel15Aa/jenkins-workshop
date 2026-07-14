pipeline {
    agent any

    stages {
        stage('Check Version') {
            steps {
                echo 'Checking Terraform version...'
                sh 'terraform version' 
            }
        }
        stage('Initialize Terraform') {
            steps {
                echo 'Initializing Terraform...'
                sh 'terraform init'
            }
        }
    }
}
