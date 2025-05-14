pipeline {
    agent any
    triggers {
        pollSCM('* * * * *') //Polls for changes every minute
    }
    stages {
        //Stage 1: Build
        stage('Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Description: Build the code to compile and package it using a build automation tool.'
                echo 'Tool: npm (for Node.js projects), '
            }
        }

        //Stage 2: Unit and Integration Tests
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Description: '
                echo 'Tool: '
            }
        }

        //Stage 3: Code Analysis
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Description: '
                echo 'Tool: '
            }
        }

        //Stage 4: Security Scan
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Description: '
                echo 'Tool: '
            }
        }

        //Stage 5: Deploy to Staging
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Description: '
                echo 'Tool: '
            }
        }

        //Stage 6: Integration Tests on Staging
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Description: '
                echo 'Tool: '
            }
        }

        //Stage 7: Deploy to Production
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Description: '
                echo 'Tool: '
            }
        }
    }
}
