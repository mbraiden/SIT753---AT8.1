pipeline {
    agent any

    environment {
        DIRECTORY_PATH = "/home/mgbho/uni/SIT753"
        TESTING_ENVIRONMENT = "SIT753"
        PRODUCTION_ENVIRONMENT = "MGBHOCKEY"
    }

    stages {

        stage('Build') {
            steps {
                echo "Using Gradle to compile and package code, from: ${DIRECTORY_PATH}"
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Running unit tests using Jest to ensure code functions as expected"
                echo "Running integration tests using Playwright to ensure different components work together as expected"
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Running SonarQube to analyse code quality and ensure it meets industry standards"
            }
        }

        stage('Security Scanning') {
            steps {
                echo "Security scan using OWASP ZAP to identify any vulnerabilities"
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploying application to staging environment: ${TESTING_ENVIRONMENT} using AWS EC2"
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on staging using Playwright to validate production-like behaviour"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying application to production environment: ${PRODUCTION_ENVIRONMENT} using AWS EC2"
            }
        }

    }
}
