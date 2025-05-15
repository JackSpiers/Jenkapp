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
                echo 'Tool: npm (for Node.js projects), Maven for Java or Gradle'
            }
        }

        //Stage 2: Unit and Integration Tests
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Description:  Running unit tests to validate individual functions and/or methods, and integration tests to verify that components work together'
                echo 'Tool: NUnit, JUnit or Pytest depending on the language can be used for unit testing, integration tests through traditional TestNG or open source Keploy'
            }
        }

        //Stage 3: Code Analysis
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Description: Analysis of code for technical issues, bugs, and quality of the code'
                echo 'Tool: We can use the Integrable SonarCube for Jenkins, specifically the Sonar Cloud. Alternatively for github sided we can use Codacy'
            }
        }

        //Stage 4: Security Scan
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Description: Scanning for Security vulnerabilities inside code and dependencies'
                echo 'Tool: OWasp or Snyk, alternatively for github sided we can use Github dependabot for dependancy vulnerabilities.'
            }
        }

        //Stage 5: Deploy to Staging
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Description: Deployment tool inside a staging environment mimicking a production stage'
                echo 'Tool: AWS for common deployment, Azure or alternatively Docker for containment.'
            }
        }

        //Stage 6: Integration Tests on Staging
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Description: Running integration tests within our staging environment to check it functions as required for full production'
                echo 'Tool: API Testing through Postman with Newman, Cypress for good end to end testing. Alternatively Selenium or Keploy.'
            }
        }

        //Stage 7: Deploy to Production
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Description: Deploying the application to the production environment after validations are complete'
                echo 'Tool: AWS has a tool called AWS Code Deploy, alternative for container production pushing tools include Docker, ansible can be used to deploy automation tools in jenkin.'
            }
        }
    }
}
