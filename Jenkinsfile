pipeline {
    agent any
    
    parameters {
        string defaultValue: 'main', name: 'Branch', trim: true
    }

    stages {
        stage('Get code') {
            steps {
                git branch: '${Branch}', url: 'https://github.com/Uncle-Moris/jenkinsTest.git'
            }
        }
        
        stage('Build App') {
            steps {
                echo 'Complie code'
                
                echo 'Run unit tests'
            }
        }
        stage('Deploy to test env') {
            steps {
                echo 'Deploying to test env'
            }
        }
        stage('Run UI test env') {
            steps {
                echo 'Running UI tests'
            }
        }
    }
}
