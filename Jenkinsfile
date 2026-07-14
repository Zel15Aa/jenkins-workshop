pipeline {
    agent any

    tools {
        // Кажемо Jenkins підключити інструмент Terraform, який ми налаштували
        terraform 'terraform'
    }

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
