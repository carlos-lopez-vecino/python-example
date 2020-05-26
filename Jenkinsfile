#!groovy
@Library('shared-library-devops')_

pipeline {
    agent {
        kubernetes {
            label 'cloudformation'
            defaultContainer 'cf-deployer'
        }
    }
    environment {
        DATE_TAG         = "${sh(script:'date +"%Y%m%d%H%M%S"', returnStdout: true)}"
    }
    stages {
        stage('SonarQube Scan') {
            steps {
            }
        }
        stage('Docker build') {
            steps {                
            }
        }
    }
    post {
        success  {
            echo 'Send success email'
        }
        failure  {
            echo 'Send failure email'
        }
    } 
}