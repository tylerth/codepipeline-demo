@Library('github.com/releaseworks/jenkinslib') _
pipeline {
    agent any

    tools {nodejs "node"}

    stages {

        stage("install") {
            steps {
                echo 'Installing dependencies...'
                sh 'npm install'
            }
        }

        stage("test") {

            steps {
                echo 'Testing app...'
                sh 'npm test'
            }
        }

        stage("build") {

            steps {
                echo 'Building app...'
                sh 'npm run build'
            }
        }

        stage("deploy") {

            steps {
                echo 'Deploying app...'
                withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'aws-key', usernameVariable: 'AWS_ACCESS_KEY_ID', passwordVariable: 'AWS_SECRET_ACCESS_KEY']]) {
                    AWS("--region=us-east-2 s3 ls")
                }
            }
        }
    }
}