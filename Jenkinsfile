pipeline {
    agent any
    environment {
        DIRECTORY_PATH='F:\\Deakin\\TRI1\\SIT753\\8_1_C'
        TESTING_ENVIRONMENT='Deakin-testing'
        PRODUCTION_ENVIRONMENT='Tran Mai Phuong Nguyen'
    }
    stages {
        //stage 1
        stage('Build') {
            steps {
                echo "Build the code using a code project building and management tool - Maven"
                echo "This step compile and package the code"
            }
        }
        //stage 2
        stage('Unit and Integration Tests') {
            steps {
                echo "Unit tests by using Jenkins JUnit plugin"
                echo "Integration tests by using Jenkins JUnit test framework"
            }
        }
        //stage 3
        stage('Code Analysis') {
            steps {
                echo "Check the quality of the code by integrating SonarQube"
            }
        }
        //stage 4
        stage('Security Scan') {
            steps {
                echo "Scan the code project to identify known vulnerabilities and security issues"
                echo "We can use SonarQube to scan and check for vulnerabilities"
            }
        }
        //stage 5
        stage('Deploy to Staging') {
            steps {
                echo "Deploy the application to a staging environment: AWS EC2 instance"
            }
        }
        //stage 6
        stage('Integration Tests on Staging') {
            steps {
                echo "Run integration tests on AWS EC2 instance to ensure of performance and usability"
            }
        }
        //stage 7
        stage('Deploy to Production') {
            steps {
                echo "Deployed to AWS EC2 instance"
            }
        }
    }
}