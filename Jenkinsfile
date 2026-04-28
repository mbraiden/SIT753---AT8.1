pipeline{
    agent any

    environment{
        DIRECTORY_PATH="/home/mgbho/uni/SIT753"
        TESTING_ENVIRONMENT="SIT753"
        PRODUCTION_ENVIRONMENT="MGBHOCKEY"
    }

    stages{
        stage('Build'){
            steps{
                echo "Build"
            }
        }
        stage('Test'){
            steps{
                echo "Unit Tests"
                echo "Integration Tests"
            }
        }
        stage('Code Analysis'){
            steps{
                echo "Code Analysis"
            }
        }
        stage('Deploy to Staging'){
            steps{
                echo "Deploy"
            }
        }
        stage('Integration Tests on Staging'){
            steps{
                echo "Integration Tests"
            }
        }
        stage('Deploy to Production'){
            steps{
                echo "Deploying to production"
            }
        }
    }
}
