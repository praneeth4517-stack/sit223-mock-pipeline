pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building the code using Maven to compile and package the application."
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo "Running unit tests using JUnit to verify code functionality."
                echo "Running integration tests using Postman/Newman to verify components work together."
            }
        }
        stage('Code Analysis') {
            steps {
                echo "Analysing code quality and standards compliance using SonarQube."
            }
        }
        stage('Security Scan') {
            steps {
                echo "Scanning the application for vulnerabilities using OWASP ZAP."
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo "Deploying the application to a staging environment on an AWS EC2 instance using Ansible."
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on the staging environment to verify production-like behaviour, using Postman/Newman."
            }
        }
        stage('Deploy to Production') {
            steps {
                echo "Deploying the application to a production environment on an AWS EC2 instance using Ansible."
            }
        }
    }
}
