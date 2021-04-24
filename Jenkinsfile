#!/usr/bin/env groovy

pipeline {

    agent{label 'nodejs'}
    stages{
        stage('checkout'){
            steps{
                checkout scm
            }
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
